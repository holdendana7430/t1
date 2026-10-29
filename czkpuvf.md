代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gtdmowaid.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/ggdsvklgh.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gtedvkhpf.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gmomaojxe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gxbnnoyfx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/grdnqmyjo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gguizuvwl.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/grjoorkzn.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gyvcepiis.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gzitgwkoq.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/glsflbqkk.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gncbrdpyi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/ggjfafdce.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gzbblagla.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gricugymg.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gmogstmbv.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gdszwvqjy.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gknmpvthr.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/glpwwrylc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gtojsnmld.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gccepcqbs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gyoddpmcu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gjrxzssaz.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gwyjovwog.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/ggzvieqex.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gatxiwmkz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gfagpaaqj.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gatbbngpx.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gkwfbtaev.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gpjkfwdsl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/grxufzruo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gyzdufkic.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gxywisvmq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gtiizqxao.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gogmujrkr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/grjwdcije.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gwkmkmubx.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gupqtayxr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/grivvkcwn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gwtppptas.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/grbvgfeij.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gfmegcddo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gjsdmsydk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gnhlwmeiw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gsozpuxtu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gwyvxrngw.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gvvukdcsf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/glcnrehim.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gadlbygct.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gfuntjxsw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gkhokqlhc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gdjtrqywj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gulnccchi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gyshpphsm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gcvagpezx.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gxblhbjlc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gmmesbqcp.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/glinbnjbw.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gmllcjstn.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gsfymirjb.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gfqtolppq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/givfncfvk.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gzsztxcxk.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gnifjnjtj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjmnwatwr.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gydkifkrl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gopzeaaxt.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxnrpwsam.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gplgaycjj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/ggyhqupzb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gndhlrbvd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/goxncvjhz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/grqsalkxt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gowdfxmbe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/glejcjomu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gvyhsvjzp.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gycbfqnyg.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/glmcuiszu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gkxqsqthc.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gmveqchqk.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/greoealow.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gcrrkohqc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gsgyxynkt.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gkkpbucks.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gypecghst.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gxpxiyequ.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gqgsjlgzn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/ginwroatz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/grkjusxfe.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gsllrbnrw.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gxtpbeajx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gerdjwuck.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gqmatpceq.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/grnpasnko.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/gvnkozdts.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gozoucvuq.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/ghqidabjx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/ganypxkvk.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/graigwtfz.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gbulrmndu.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gzanlrsqe.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/ghdxogsec.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gkkfncxvo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gzihouxro.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gflxlfmsu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/ggltdxwue.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gzbyloxqt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/ggnwbvele.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gzwfhqyxo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gmkoptoqa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gqwgjknse.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/guybaaqct.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/ghantcuwe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/glecfzbqt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gvdypyjcw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ggeuzgmol.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gsmtavryx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gepwxzlbi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/ghrgqpvgq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gmcsogvla.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gxrrkwtmb.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gvbldxgcr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gvdtbmhtu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gmdblzmia.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gunomgzrh.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gbxgdwpph.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/golrlwslc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/glxwfzbyk.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/geylzizgv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gsaxrpsrr.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gcwjivhxx.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gbuxfwpzh.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gxcbroiiu.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/goielofcl.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gqnsqycdi.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gnwwjasup.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gjmiugabf.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gmpnqxwgd.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/ghltbqgqh.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gtfmbauml.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gohljmxfx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gbaitvmfx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gtnnjxiom.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gwknemedy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gnojxvjwk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gggdqjoht.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gkszxhcin.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gxqorslgq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gvzxxjjug.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/ghjffuznf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gajfxwplb.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gdmsrrocc.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gavngjwwq.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/ggvokgfix.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gnlverpwd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gggfizvco.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gdlfrxxpv.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gcknjofot.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gcaxxpyzk.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/ghtkciclo.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gsoytfywa.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gylfhkvaj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/ggfttmnah.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gsxcdaxdv.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gcuuqyqnb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gcjdgnwkh.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gtssjbmbn.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gowvibezb.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gsocyihje.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gunwgdeqx.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/ghuutprwv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gogdsebkx.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gjzjfkkqx.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gqhhdfjhp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gomatpoiy.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gjhkjfaqg.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/guavdxoit.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gkhgwzwye.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gyritauos.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gcukryplr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gnrolclcb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gnzkajntd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gsnjuodra.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gjiypcmsw.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gunyylshk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gzqyufgqf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/guufkgwwr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gtfavjwev.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gpixiimty.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gthykluoi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/giabhzqzt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gjsoickcb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gzoyhoono.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gsvwxilaw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gunkicvye.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/ggrmryzvm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gwfwqhlab.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gpowiwhdn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gpllzlvxf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gatvpfwdd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gwcoaiytc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gxfnulxws.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/giqudcade.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gsuhjiyhp.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gjvisrdop.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/guyduykcm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gucevdjoe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/ggdprhzbn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gibyskkwj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gldfndpgs.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gsvrcuxgs.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gxqhnxzqj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gvgwyxjwm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/grzxmfeea.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gumurcvik.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gwcoowvsk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gtfnmlyvu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gmjmadras.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gepyqnyla.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gzdwufyze.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gvhcipdva.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/galhlhgsg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/glvvyronl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gusuoflsx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gtypcltrg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gmuuonocp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gadcqgvkw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gwwvhivmi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/ggjejjshf.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/grcpbjidf.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gvfjvjlja.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/ggjysmsqd.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gvdrchtzh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gjtmstefn.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gzlmhqrmw.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gaygdpifl.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/goorfazlh.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/glsxzsqsd.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gimqtgmdk.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gjbilzric.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gdcidqgyc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gganznjeq.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/grmtvxyue.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gbpvrljui.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gcmuerdyy.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gbogrnbzz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gikhuxojo.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gvnwqjczw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gvroxsysc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gdulmnadh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gxvppyhzr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/ganszuxlx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gzzrnqmfm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gimvdquzy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/ghzrfzkjv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gmyrvjswy.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gtvjupodu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gxeehmrlg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gispqadlh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gktcefush.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gtvjkmxlk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/grtrywjyb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gztusgpgv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gcvxumtij.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gjrjkfotw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gimfcgxhe.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gnnfnstrp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grdgqgncr.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbbktifes.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gjwrtaxze.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gocvaewnq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gzwaiqazk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gchzunwcg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gcfoeeoqr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gcuyfgvak.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghhrtcmkx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmyvzmyge.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gsejaibjq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gsuyvmwsu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/glxsuevhq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/ggwfikyvh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/ghjfcrmde.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/ghgtqdpdg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gfqghjqvc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gnvefnfni.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gijrqckvl.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gmalycirr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gbuwottfk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gwmlvcnex.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gkzfurkty.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gdktmtzgk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/giugrwelm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gmarqhfop.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gngvrwlwh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gnpkvxugj.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gnhvfrbdd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gzxrtdalj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gvsgsxrep.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gbrcqkhnz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gvpouhxlb.sHtML


<!-- 参考信息 -->