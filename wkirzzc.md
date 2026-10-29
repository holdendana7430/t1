代发 wailian999

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gjekrtjgn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gbmjmymev.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/ggrohalxp.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gupbfkihn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/giqcrhaxa.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtzvnigbh.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/ggftbdlof.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gwmgeqygb.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gzrurvlek.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/grqduqwbo.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/grgodgnhj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gyotkjohf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtirbtlqh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gtwvnakql.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gpyhfqncq.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gqqvjxkuh.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gwqkhnmjc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gqvhjjfxo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/ghxlbydei.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gnltdatqx.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gxvfyykvw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gmdxzxbxs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gmlrhtkov.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gufgwncfl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gpxnipxtj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gvnurwcyb.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gpaahifby.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gibhjdnlv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gwzbxidvi.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/genaxuxas.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gzgvjrtzs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gcxarbgze.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbsemfyij.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gtpakemct.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/ghlzbegnh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gojbiiqcu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/goylwasaz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/ghhaoschw.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gafneepfv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/ghfeoyfwa.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/ghaixkpvm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gqnqvubqr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gpldsunsz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gvtaxbpfu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gsuufuyoh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/grmvjdtkv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gptfgiykj.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gcrepmotw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gcqnurhtr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gvpcznjon.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gkhimhewg.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/glaaydfze.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gubhotera.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gdyexrtsq.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gjteihicj.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/geletcpzb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbvtagjwk.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gpzndphkz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gskcooodd.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gonpcoowc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gdnzvidqa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gxfirkxtd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/glybkhfwb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gdkabaemv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gdwrvinqm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gplcjsjuz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gvlzwugie.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/geolkyyzq.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/glijirhoo.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gfxzctywh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/guiqxdsxf.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/ghyirhigi.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/grflpirnu.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gxsitnusc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gamqwsave.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gsyrmlqyr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gwsjozqvd.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gwqrlrdyx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gsevakfth.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gimiupopg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gmoaxjuaq.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcnvqliog.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gtqdyyuqu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gphxjjddi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gamngcopc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gthklcbsi.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gleecxabq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gaoozydqm.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gzybnvxap.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/glqtwmoux.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gpjafamcx.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/guaizdwrv.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gfdgtlbdd.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gruyskaou.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gjdoxxyzm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gilijkjnu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gklbpgzik.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gvlxosked.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/giwaoeyxc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gfmuhamhk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gprhdswhd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gjwewdgbc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gqzhekgwz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gucrttxgw.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gjwcsxers.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gjbdnxkaf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gdhrskqid.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gtodgszjr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gcduokhuq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gnczyqzat.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvomwcec.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/goyyveyyb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gbpsregev.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/ghmhctyoe.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/goszpvjdi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gtwonteho.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gbnviwozn.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gxwgxldzo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gupwnszvm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/germznpgh.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gunwsxnnv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/ghjowvlph.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gvleyiqbc.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gngejnooj.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gwherilug.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gxctkoqxq.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gevpcorbp.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gkvkhyibx.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gflcfhffr.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gdtltnrnr.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/grxeaessv.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gdpxgvfvd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/glhwyebew.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/ghqztevcl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gzbchnlfm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gragavpbn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gmqkpfxpo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gqbltidqd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gtkfzjvmo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/grhaxkloj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gdmqjwkps.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gfodqvmdj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/grcegpfwb.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gqcvbchkk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gybmtnuof.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gnhipltzj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gweohlhvg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gmakprviq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/ghczwidwl.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gqjxdxcdh.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gwliawxpe.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gkqabpwrs.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gptakqgxk.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gkjivuxks.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/geftwdfyx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gvycgklgd.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gwddphxks.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/geqolerqe.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gpcmrzglm.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gabacyuae.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/ggzjdfbrs.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gyuvbutsj.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gvgnfivwl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gknohnawi.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gogajshhm.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gwjagoswq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gcvzchnta.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gjqhyurrc.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gtucdcpej.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gahlydsge.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gzhhazuao.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/grmwidfkp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gsiobpujm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gujgenwzf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gbuxhpdoi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gznmjaqhe.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gpoingvjs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gzitdbwuq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gbnpwsbde.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gtnpqdmwb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwnoiwsya.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gipwocfwe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gjdmuwltn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gshulrdst.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gwjlnrhle.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gsyxyutei.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/goepohhxa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/giuxmioek.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gqvyhdoqf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gnxflsgij.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gdczrjqsg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gjgllzqen.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gylcipked.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gvwgbgmth.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gjthafawc.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqorfiswq.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gqrhvcoqe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gjzjxeynd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gewibdvgv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gvrctvkga.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gifebznax.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gbrrdrsvj.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gnxakyvnn.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/grismbmaf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gilzesdqu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gxsiubhqe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gvhnigqwo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/giihwqxbk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/ghruwlksd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/ggnjklbax.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gbrnwvqlf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gvazpzivj.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gegmshgsp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gupsxopyh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/giqqrxiip.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gnisngqsu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gaountvgh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gqfucgsjq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gpudlttst.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gvpzccfcg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gpfxrqbxb.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gopaxbjwc.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gapmojyyt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfuxtpdif.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/grlwalugp.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gcugoxnvz.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gwbcmnzld.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gezhuigpr.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gwsyafitd.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gfvjqqlwz.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gtmjluibd.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gyddcdorc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gncwrrgku.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gprdizwhv.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gcypfosxy.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gxmahmvtt.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gusjvtxek.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gnwjwlury.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gafdatmsz.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/geyrkibxf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gjtdygusi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gxjfidapm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/glqtxjqnd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gygtozdgg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gaqeqhhzw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gxenvamds.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gojfnbbtn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gdcvfnlaw.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gdfrqbhor.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gxabyoqzm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gpfyxuvlw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gydegggdo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gmgawwnxl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gkagtxngg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gxbbuddsz.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/ggnuzdadz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/guzcsatap.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsohwllxu.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/glvxgggfr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gflfgsndj.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gckskurql.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gmwjstlmm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ghcmaaiik.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/ghutnskhn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gjyoexmau.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gnvqqayhg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/grquieumm.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbhhqsrpn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjpcjjsbs.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gywxpxdip.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gjsnvsmgy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gqhoepftk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/glavxqzhm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gzajlcdfi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gzvbavlqy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/goimozfhu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gugzltqah.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gulbxgmsh.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gtepfbdpa.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gkbhotmwp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gsyttutab.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gteofuuls.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gglewvbfq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gdelkdqcf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gaetkjpjx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gtzqmlzqa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gnlravewu.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gkhdrasgz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gvnkjggxc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gdplshqpg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gofdlxxdf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gaddwjobm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gwcouhctx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gwosmwsdw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/ghzetkfff.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/ghcvpvidt.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gphccazwe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/ghmlndqyr.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gwaigdzom.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grntsijeu.sHtML


<!-- 参考信息 -->