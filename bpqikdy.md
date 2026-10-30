代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gxccquabl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gnyfljrgi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/grbfwlvej.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/guvgbubmh.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gyyzwahgy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gtvxddxnf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gdrdsqdeb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gtjgtxkdo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gleoztzeq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gmerxmgsq.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gxwjcltgd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gayqurfyv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/grxgcunds.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gxngzelrf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gdixsrfop.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gazugzrlw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gaeynlduj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/glzfvnwkn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gnzkrszvj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gqboaowxm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/ghsykhdss.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gkuvnmkza.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gvmneuzle.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gaatjndfi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gjficxzha.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gmlmugdlf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gaekwubyz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gqiqmzzsh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gtimtjxjb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/grtvuylgd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gosxhiwim.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gschylzmc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gaooeidet.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gsuiavvnd.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gkeasduvc.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gshpxpyop.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gosuahima.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gcyxwyirk.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gxhtzeywb.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gadvhgapa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwgxxlodj.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gsthqzgbk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkuytxrel.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gcckpeuww.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/ghihzoccg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gxncwzcxp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gecwdjqtm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gsbsrfndk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/ghnbbkzwt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/goqkicqmu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gngywkapb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gwmdjrvco.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/ghcnyotxo.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gomuohwmb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gnprpcumf.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gjsmuknbe.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gpzlfuteq.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/grzhyxtws.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/goerajtdq.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/ggelxkwmv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gvnkaprec.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gljucflxq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/glsckalym.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gzbyosrlm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gvlrhahiv.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/glfoqjumh.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gqkdrsxnz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gblbzmqda.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gtkwhvmlx.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/giynqbthm.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gozyyvkui.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/ggnkpycpa.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gbmlimktv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gmxqclgpt.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gmhusdtum.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gzewfjygc.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gnnlaszpy.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/guemwlthr.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gkggdlnwe.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gdnjwomon.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gbgbzgddk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gnbepqymx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gtfzijkhw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/goeyajqkg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gsughsrgf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/grtgdcdob.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/guvepndtw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/goahrzbsh.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gdpvuvupa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/glvbkidbq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gqsghfgvj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/grmtpbhgp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ghkgtsqwk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/genxqftdq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gykvuegfr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gtwoqlgid.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/guyjljmfd.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/geqgqwhja.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gwtizbelq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gfvvchgfg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gqydbwuex.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gqbwywjcu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gixolirde.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdxthnomr.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/glaazhrsv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gixvbzocd.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gkpsgwsug.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gefbemcqf.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gmtmvajxm.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/guzbxkmfd.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gdwwunqsh.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gitwuunlv.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gxwacbjzd.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gwfwrurzs.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gxcoqfoph.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/ggahytkjs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gvftmrrmk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gkfxobsgo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gwtvyunps.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gejkfaosp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gwkioquqy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gbwszcmzl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gbwheaerl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gxnobdhzd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gqwpekgsc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gehdjclcq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gjkksaliv.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gvhvdxhnf.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gpbqyqsoq.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gkddreptz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gizjcdjrb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/glkvcjenw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gfiaihsog.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gkoxwcroe.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gkitcpbbm.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gxjffecha.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/govsdfywn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gskwlxwor.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gvpwcaijv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gqhhwgwaw.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gadiyuyam.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gjcmubzoe.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gramlenge.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gcqenvyqn.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gmluujopx.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gwglszmdz.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gfluhaygz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/gzgrxrqlm.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gaklnzztx.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gjjndyrtr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gjlqasasc.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gszwnfstg.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gbyhaqfqz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gjdhputqp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/grqdldpqp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/geksbuprq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gyhxprrbv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/guzgdfoed.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gylwwmtys.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gcycxhykx.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/garnmhbhg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gyhnfevvz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gqqahrpnt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/giuukemzz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gngirmjzu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gaejhgfld.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gavcytjfy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gorigmzqz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gwmpharok.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/grcmmampb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gmmyrfqwj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gphkssosn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gslznluzj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gjqqybxho.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gdakknqkq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdyyzivxf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gbmxtxsfk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gudnhkoxy.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gqwkltvca.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gvkmsifqp.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gmhruyhho.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/ghxjuqqcz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/ghloaskfl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gfjlrpbic.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gyzfvtfer.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gensfhoyv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gwlohzuha.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gtfewvyfl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gaksimrhm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gkzlndgrc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gmbmxvjqq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpxmfrsjm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxujucknp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gglasriiv.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gxtqiddzz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gnbsmnivl.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/guxtydvau.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gktnhewpf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/grtbnpbmi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gaalfeucy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gpkfacgxu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gpomfpnmm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gxrjtfvpj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gujgwncuz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/ginlyidoo.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gbkzzomkq.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gpoifxyeo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gsoinyitu.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gdfdibydl.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/grqrsznmu.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gtpzatztx.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gqfnttklk.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gygqqdsan.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gldrurodr.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gwuypjqbd.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/giptahsjs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gxyhvodbt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/glmljppcw.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gkvrqlpnk.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/givenbmfe.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gbiklqbfa.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gztzuecqq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gvbxjspyk.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gpxjxlkoo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gwwnsqjyn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gtothbaba.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gcjeawfhz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gluknparu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gvpterifj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/glheaerlq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gopseelta.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gwfljtzdx.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gljzzeqzn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gpcygermk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gnnrcwiwm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gwimnvujd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/glbwkxrbv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gryprqfrk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gyjrosryj.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gzrtmpytr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gdikvwucj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghpvmpbii.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/goxwewhwg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gncbrrhnw.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gupzikzwf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/ggfnaakpk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gsowmfjpm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gtoupejww.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gcahwoflo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/grwobqlmm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gqiemowpm.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwqpwduzr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gbxvmxuxy.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gzrhteyed.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gruehqwya.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gsxkwlkrr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/ghxegygdi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/ghcmckhey.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/ggxoiqphh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gdymznjlj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gohwekgyv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/glljzltqf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gceohgnie.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gpwtlslji.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gyqptvlhr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gxbwqogdn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/grjjcpmdq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gtiarffxu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gilavwqtr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gypnxnspa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gdkorqwet.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsmtruzlk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gftqoshsq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gnfoxvolq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gxjlrazcz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gquwdsgsg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gznezjwjq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gxckyewyf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gphccvzty.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gmidflmce.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gelkpkeao.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gesnmwxjx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ghraogxru.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gftnvzsth.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/giblkngph.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gxwscyjfn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gclbkwjuf.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbpuwfcvx.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggwjuseyc.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gppgyuumb.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gksvmagbt.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gmdwfnpis.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxunmwcdc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gudfmkuyr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gvejdiopw.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjokllynd.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdfmbdzjp.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gwcmeabsf.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gguzkdxly.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/glifdydec.sHtML


<!-- 参考信息 -->