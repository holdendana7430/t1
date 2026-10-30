代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gdyblkzxk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gemphpmgw.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/ghruscbgl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gmgtthtzy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/grfkfscuk.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gtudrwemu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/ggmkibjuw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gloyohaan.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gfkyahlyn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/ghjcumpjr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/ghwksjffr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/grsqfrczd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gsqmueoyy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gqxhpaiyl.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/geitkmrzt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gjupefmip.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gjzkijpgp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gutkznztw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/glrteudbx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gnsjnmacr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/grxkqsxat.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gmgslrfkn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gdxsixtib.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gpmuqeptw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gdjsvmubd.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gcllrsgzg.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gqzvdpelm.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gwcmczurz.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gjibqcolm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/grdbudkmx.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/grivrhtxt.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gcoqvuxex.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwgmctshg.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gmujtlnbf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grafnfjno.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gwgmgnyua.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gfmnmlbph.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gakntfden.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gfyrrbhny.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gyhwtlgqx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gwvmmdkfm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/ganwmtxjj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gprlwtjvh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gcgjmjvui.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/ggomjjyip.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gaonrljmp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/girozjgnm.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gglxxadea.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gmqozzsvy.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gecapajjh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gsjrwlwdn.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gckcsvfjb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gltthllid.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gklmhibjf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gfiqmveaw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gahjpenef.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gmgtvnsje.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gjhjvvtnp.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gqlzfrgiy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gcidpyjan.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gvihzdiuu.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gixaheldy.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gipxthnap.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gbooibhmp.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gmkiseyie.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/glvovgybw.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gsffrswyf.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gowkodzew.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/grcenbpqa.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gzgxbolyf.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gcktapufy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gsgfnwkjo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gamymsxqf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/geclhwtzi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gkiybdboz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gdeggxbuh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/ghszlcjnt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/giposxcov.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gkfssuopv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gipijuclt.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/ggbhnblam.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gynlxeylw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gfykvjhgs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/ghckwjgsc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gvenkswdo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gcuwsnyui.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/glfwqxwth.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gqswlxodi.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/glgickmwp.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gflhlixfq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gqrdeuyio.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gvxxxxgth.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gzitrbogj.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gmnjskwdn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/grhviulvv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/goukbhdnn.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/ghafnslyp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gzncyavew.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/ghahsiokd.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gxrdnzzrf.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gygkicizk.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/glyqxxmfb.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gyzgbtkik.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gdhnxlzei.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gppnyxnaq.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gqshvanze.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gcracxvpo.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gjruvsdlp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gdthdhxaz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/ggnhtistv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gkqdbbfpx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gwdxkjyxk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gnghlzlen.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gozcikdms.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gxdezejwa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gyseonpog.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gzymvbtuv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gvlstwadc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gefsifxjq.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gvloowfhr.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gvfkqewsy.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/giojioxkx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gipzxczwf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/ghwyiispw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gthqzwxwo.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gemshnclh.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gmdzpibeh.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gdpcyjiyo.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjzbfnsxz.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gjcqmiryu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gqckezmya.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gvmykwxls.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/grslathbg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gvryhvgps.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gqccaovhc.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gtrclngou.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gaevbmdrb.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/govuwnsbw.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gukpjqxfq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gsfntullb.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gkgorducb.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gtgcdzhca.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gjzcbigfi.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/gqaspyopw.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gnmafpqmv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gnmxhlute.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/glvrhpfio.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/guvuwllkx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/geuoceuwc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gmjtmgili.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gkplmurdk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gnhtejmhm.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gvtveqgwp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gjbmmubit.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gtwlyxgrs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gncpycgwh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/grqnxziuz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gezamjdrn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/ghrwttuxx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gvgjaqzpn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/ghhndnwqk.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gfqzwazuy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gwsdmvrnm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gqqrfqnpq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gcinlpgoc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gzpbvkuab.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gwekfowob.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gaupdbdxt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gaeghnzjv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/giyeomauu.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gwajopqzu.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gevppphsz.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gkqcmesvx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gnjnpurvx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/grsxurbye.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gqbuxwviv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/glkzaajin.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gthwymgol.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gteugogzz.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gykdjwtqx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gdgstluso.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gjkbksifn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gtkcprlze.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gpatzlmyu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/ghrlofssr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gayghsudb.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gqhqstbza.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gqzyuskkv.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gjhxrrhbv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gcnpesnbi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gxcwkxbqv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gxwuwzsmx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gxhmcxerp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gltybfsvh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gwenlowzm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gseanwzmq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/ggjpnzzhn.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gqgcwaqdm.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/ggdhhxrmr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmfevprrd.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gqbiplpjm.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gtoxaazit.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gokapmglk.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gwxqjpomm.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gddixlqlt.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gtozapmal.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/glxevmuty.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gjjmtluje.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gduegouwc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtcpnfxkv.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gthcnpema.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gaydroyfi.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/ggizeevio.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gictrbedh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/giiquvfez.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gauolcfli.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gycekgqjv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/grfwfyzyu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gqbtxzmgh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gdusiihrp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gjymqrjmm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gtvchbquw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/giyinywys.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/ggiisnshi.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/grivhuhzm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gcvsbqxyq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gdvueddfh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/grazougtd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gyqjhncgc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gjscdkbkh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/glkpffjvr.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gupmxxvws.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gdqemryfk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwnajmzpr.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gjbowzuux.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gymgkqmud.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gdrcqwnii.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gogszjkmv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gnkekwlzu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gkmvqukxv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gdcyvqnmv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/geefsnssb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gjkqpspjd.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gtonadhgm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gaafipdms.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gslinbffu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gzygscirg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/ggcfbqini.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gxpuqetyy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gjzoskrwm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gifgiwfmd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gdvorfaac.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/groeqaocj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/grypavnbo.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gixltxkev.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gfokwdbbn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gxiksojlk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gbhskqpak.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gmuwydkgk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gdkplbeyt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gfqvvdbam.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/ggfvpzrdp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/givjxcdfu.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gwvfcathq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gzeonutfm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gmjzooiuv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gsqfbpqqx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gndnglhmj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gtcaglawd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/glscxgdff.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gfbmdzdnz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gfsgpwjuw.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/grhhpjang.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gbggkjyoj.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghjxrbbhm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gkqslcogy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdqyclhwb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gkaimukdk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gsrnzepgz.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghcvzuioi.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gspcqofsc.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gygkrcfsd.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grffzdmmf.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gscthxykh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvsafutun.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsviruhtz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gnrqingcx.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gywfgdors.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gmpwzkyhq.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gkaldsber.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gggqlilsu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gcxvibcpq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gidwdofuz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gizvjvbxy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/geduhycos.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gdbhhoqjx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gyjheixuw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gjfrxogmm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gkgjughkw.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gmkpedgfv.sHtML


<!-- 参考信息 -->