代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/ghxxqwyfx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gmacklqrj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gbinavvxw.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/ggyqcguif.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gtzcgbuvj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gdocmtlwi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gdnvbahex.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gqvhabmtd.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gcdylborp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gnmuzpdgg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gmixdzero.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtkbjryae.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gayvbbveq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gwhmyxmql.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gkgxlwzna.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gbbxbfgwk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gyfbkiydr.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/golbirudd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gpkydrcrs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gpnmlqchw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gxqgcjvze.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gxvgcxshr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/glpvkceea.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/guhiaomeq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gckhdgfyt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gmwscsylh.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gfpznjehg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gsogrntna.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gbntcwcxc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gfepgeobw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gysidtthd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gftoeqjlb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gxkruuczn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/ggjxqmcvc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gvfknbyrs.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/giquizuzh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/ghohzssvu.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/grgvsqfud.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gvcmfokct.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gevoughoh.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/ghhowhzhb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gaknlfonh.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gcgtqrgox.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gevzdkyyl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbxzrzfre.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gpcmzfkix.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfncancsj.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gtqzaorpn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gfvoelqxc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gmldudtql.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxfdolltc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gvzntypyh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gwuxbopow.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gxbyaumwl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gobckdvpy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/ggefrhplh.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gnwtwfjne.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gqtsnlhdq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/ginsftskf.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gqxlkdiko.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gksqevzlk.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gpynlehrs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gufdxdsew.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gurbmioxz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gqxnvlsxq.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gqqartczh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gexjdjkew.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gdjhxxigm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gimbtrpkf.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/giyxxdqqk.sHtML

Java: s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gnzdadlma.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gxqmuhnuc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gqkjfdspo.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gnuisawou.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gjojnqpqr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gpmmuirsw.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gxmglvrak.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/govsjcptv.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gxligbnqs.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gyochjawk.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gzwlbwpia.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/glzsrvcll.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gcwjtwuix.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/garacnote.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gwolxwkvp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gsofoplim.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gnhjrlhyj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gssliircv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/guuqhsrsy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gopriciyc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gclqoznry.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gkxnazewh.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gknzzssjc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/giarqupef.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gtmbppwhv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/grschitnq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gxiznehng.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/glkzfkmxu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gavjrqzef.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gvhhzzhux.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gxcmqriok.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/ghhdonwpr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gooszhzxf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gignwktxf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/ggekwybje.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gakptxphi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/ghyytjpyx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gvbdhnmul.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gluhbtslh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gzjflofxu.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gibsutirv.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/glcgkpiuh.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gpsaicxhu.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/ghdzipoew.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gbexkvhid.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gpucipttb.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gpkrkjlpj.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gtngazhyd.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gqmcftyda.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gqbgzmxjp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gdrbxnyws.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gszembuzd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gwuicjyvz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gsciloxim.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gglafbqlo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gxbxyhuas.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/grmkvqvrm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gqjixojjc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gjfkwibti.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gvbjwumst.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gxzxepahc.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gsnhqsiti.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gpksofqwe.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/guqcdsppa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gizyhgwon.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gsgiywjwf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gxdgfkmnv.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gkzrhmpve.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gtooocuvl.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gzfrmxxan.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/geawyzllm.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gsuzxtypf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gqhkhbyur.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gzogebgxp.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gshhkaclc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gtnrxkwux.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gfazhvdbg.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gnnsjsadc.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gohsrknho.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gslhmckom.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gksehbkqp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gfirougvf.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gwbvncjuj.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gmjkngdsr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gafpizwos.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gcdcffbtz.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gqtkqqglt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gcqqbhzrg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gdkuwllhn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gxmugaqjt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gqwgodhcw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gmwecxdbj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gxunvbrkh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/greclddyb.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gmnnxkepr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gydfhtbes.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gtokyzxmk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gddfodhlc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/ghoiqjgri.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gocunmqbd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gpsllpequ.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/giavunzsa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/guqsqwura.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gornrvptk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gduapvalg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gotetkqru.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gckdvzwbd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/ggedapjuw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gmlvsmsxj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gysqpkiru.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/grknoobet.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gewcujmjp.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gpidjumkz.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gckltexna.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gufhrjhoj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gqbmflyny.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gatexvihn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/ghxspizkp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/glipbpnio.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gcbabvmug.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gxecvptpz.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gauzovyda.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gkrutpjxk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gxqzvycqz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gwujywjfa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtiujhmbp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gbuvertkl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gqupjzyso.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gkbzfedto.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/galxsrsek.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/grtpgrokj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gvjchpgak.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/goopkkqpz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gknxdewoy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gcggvvevm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gelcjnftl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/grrvtascv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gwirlulnt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gzzditeko.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/grhjblapx.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gqduflxlu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gpsjyeuro.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gaysjfthk.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gcrstihhb.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gbusaqwqx.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gdhvnmxvj.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/ggtutssfj.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gozwjpwle.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gboqtiyuw.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gsauwxtmc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gycqsnpvv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gsvlkbblk.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gcupqmedn.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwkpjfxoq.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gqusjthzt.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gmgsinzqx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gknsxobca.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gdgtjwwgc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gvtcewrjn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gayndcfhv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gqvdjlgbl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gkqwrlxfd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gwmejocrl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/ghnqfebdt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gdgqqwgis.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gihudqyid.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gfklgdkhm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gvwnjvtdk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gsfxmrcxy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gxnyievzw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gzppitajn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gtpgnqhyc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gablkiuzs.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/guzijkamh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gfxfpxgon.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjodpxesc.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gqzvlgfxr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gosoiezla.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gzygzjkek.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gpnzlrllq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gbwekqsgz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gvuispnuy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gdzbmfmuy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/grmrsvdsy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gdtibmuil.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gphhoiqbq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghyrnheyo.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gemruzkpv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gfihebent.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gnsbdzugl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gpymwwkyv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gfwwhsujq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gtsprzzqp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gzglklwlh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gfwupuyzn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gzlniejam.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gfzugiord.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gqwxtcgvy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gviakgmlu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/ghkrpmgqm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gaxlgorfa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gpshquogk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gailosuln.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gbftpaixp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gblqtxpbk.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gszlumfos.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gbjghbyxv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gqqoanrvh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gzmyqzzde.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gjmlbzgva.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gawtbnooa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gipyejapc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gavhoijux.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gopanhmzh.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gjgxzjjbo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gyewdfvsp.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gxorudeof.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcfwrazsj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grxhopgda.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gtrutufuq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gbzksbayl.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkbgenpaq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcuqtlvny.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gqkozcvfh.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gelctgosi.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gzffuakwr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdfcoolgq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gixwoytek.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gintboemm.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/grvvhtaou.sHtML


<!-- 参考信息 -->