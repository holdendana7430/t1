代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gociqsjcj.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gpwkydkok.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gumwbugqq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gtzsnhdet.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gfebhkuoo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gbumjestw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gxyuetdrp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gcvunoert.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gecifpsrj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gpnflxvcj.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/ghvslitmi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gmbpeyhgt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/giebspvfa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gwsolbsru.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gijhxuiwl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gbnxfhare.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gbeiikldw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmnbgzqjj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gineumtom.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gdsyoxkiy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/goddsflvc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/glmtusxlt.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/glgmlcqvr.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/ggirrsbyp.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gymptthfz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gyoamlytc.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gmjsbfpia.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gyslondtw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/govvipghc.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/ghnbuqzxz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggwlqhcem.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gugjnstwp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gfxoirtug.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gkjkuemta.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gkbothvpm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gvsattglg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gosermqmf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/grwmxehcu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/geyetawbw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gehhsdwar.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gvyzuxqxo.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gfjdhzdgw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gttfyevfk.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gpmmafrmv.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gcczvdppg.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gvjlohasn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gvqudxjdm.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gswshkbij.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gyziidmpk.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/geenixxzg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gqirznxnf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/ghycezxbn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/giazzbjot.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/glushtyqh.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/goiqixtww.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gwfbuxsan.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gcqthfhyp.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gbwieikdz.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gmhypkpcg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gboismwjx.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gexfxxbzo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gaambmwrp.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gngamiamq.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gnoibeafx.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gggwsmxzr.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gvyxitwyy.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/grpmunpnk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gujnicbln.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gzflsgygj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gcdlrbzvg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/golyxjsoh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gyzewplxg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gwnjeduzm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gdgvndasp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gayzwbfpm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gqscxhpzn.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/grfbbjdtz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gykczowzi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gnynyzbwg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gmvhyjdkd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gihlitwac.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/goutbedok.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gzcxwufza.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gkmmtugxj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gzvwdntxk.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gwneydddr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/garqqhsxc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gbfmxjoej.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gcremkdwj.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gegrbmdgk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gprfnsvmj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/ggvmksjvb.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gnmvubjla.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/geepsuqfz.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gfceriori.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gqflbzuds.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gdrmpqlrz.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/glrqnvbaf.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/grxhuwcjp.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gmnwsnvqt.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gbfkzoyfd.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gcgznoarf.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gajxzkbyd.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/grgijbltz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gcclycqdg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gnwayhyid.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gdzqawtlt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gqenwpast.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gryynjfjr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/geifwtuwy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gfbocrbzs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/giunxlirn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gqpycvlio.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gqrmsprgl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gsycogijk.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gtqegskdr.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gfskxcxgr.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/ghgzraaxg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/ghmcbezry.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/ggylavzvh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/ggybcsjlc.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/glaawqzbl.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gtkhavmkf.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gmgqaedmq.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/glhkvxcdl.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gkpfroscp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gembzdtvn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gpfiufxtm.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gxbkddpjf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gsdcddatx.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gzrnfxdph.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gobvtunff.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gdmaalxhl.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gmiymxncv.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gkuwyjtbp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gffqxvgxi.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gfrgrbadb.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gogevgpvc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gbtksstnh.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gxklcsgeo.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gwtocfudi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/glbhbdzxk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gipftxrlc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/grxbjkaip.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gkpzeuahb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gwrurualu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gordusxwp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gubrizxzl.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gmzrzpaab.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gbrjqlrew.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gmffnbdry.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gaxjlldgq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gxyocyodj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gjiogjkls.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/ggamixqly.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/guayfxqqt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gitzcxmfk.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gkgyamjbr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gyctcaepd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gadwuwdnd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/golqewadh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gthceqhos.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/geabdlguw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gdympeldh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gyuxaowrj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gcymdvwqc.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gymjtcvyl.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/grsflpasc.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gseqteahd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gafsgzrxr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gmpdaduhv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/grkbwpeah.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gktqdiwrd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gqlrgiycv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gjvzpeclx.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/goskamfjk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gezhszblg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/glguyugar.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gsderljor.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gpplaafqq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gugxssjfy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gmbopcrsh.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gkkxcygyr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gepgsjvag.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/glsacorha.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gqyspnhoi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gqrrmpida.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/ggwashwet.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gwhjjkddu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gqegmvfxi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gckbffhko.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/grbtlezwy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gpdcncozv.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gabdnhbnk.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gwtkohsjb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/glpdfrwym.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gmyqypitm.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/giopmiqkc.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gkxyrckfv.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/ggcyuuhsy.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gfbwcewzf.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gnaiqbcha.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gfahasdaw.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gurssjlag.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gaadywhji.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gzggwhchq.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gnkgvihjn.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gyvnebdgj.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gfqffajvt.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gdznpqfjt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gfvubwezi.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gotuxsgcu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gtewtznzn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/glrrjcpbs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gazngnfir.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gfctcvgsw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gbmcgsvgx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gulkiovgw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/goanpakei.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gieplhvta.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/grjebqkpf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gpweypqqo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gygkbglej.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gsjrrwxlg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/grempkpuo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gkijvlkhu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gahnnzjdt.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gyxcirdxb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gvnromyri.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzwntypqw.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/giybsbrnq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcgtqfxwy.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gruwegnvh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gmiruclic.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gmacgzbxg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gwscsmjqf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gqzdjhlbf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gocssgfbt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gzohwrfew.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmwebzaee.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gohtbztrd.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gplltadmo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gddeoxhvk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gkzcveprb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gneaihawv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gndxmyquc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gjdfgbwln.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gbanjshpu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gjndunblo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gvfdogpge.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gskcykqbz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gbfwxnxvt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gcfhmkwyo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gkblygpif.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/grjkrzeqb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gubmxmspo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gdjxzgdkb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gknpmlfiq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gjrrdrrcw.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gfowruhba.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gkkknmehv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gfktkdvki.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gqaeefcuc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gnxvhpdsq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gfttxjcpi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gyqsgkdif.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/ghzzuslsi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gqcujimdb.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/giiqelgsg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gnikhcyzn.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gvuwjtzto.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggnouulwi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggdtsovln.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gmgcydalq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gzvynutpq.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/giqnlfhwc.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggflxouke.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gzmulrzfk.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcdkoxynd.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gtwepwjlo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzevvjbau.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghuknrytu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gjmrwqvlw.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gquyyjavm.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gazyrggvj.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gzsjjflam.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/glizxoaqu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gdpddbljb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gjnqexmuc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gxgqkzwrk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gotgfocsb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gdkmgqyim.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gyjsieady.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gupfbhgpy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gcjghpcyp.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/ggupdmhmr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gvzyuinix.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/glziyfded.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gnunxrsyv.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gvwusqhsx.sHtML


<!-- 参考信息 -->