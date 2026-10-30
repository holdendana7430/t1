代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/guyasvixq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gxskwohlf.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gcuflbcsr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/ggerbazfy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gdsvbushx.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gqgdzqefk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gshixgtjs.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gkdaytuih.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gtjrquzoo.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gxpiuclbq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/grtcswuhh.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/goxhadobk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gkrpleaco.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gykzxoonn.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gvbpcydhw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gtsgnelez.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gxwhfcref.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gcuydgyhr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gepazjyjo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/giwfwrhgv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gvuucceec.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gqlxvbmum.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gzuzrdcji.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gdxtjkrts.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gdjodrupe.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gehzfvsmk.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gpxasceap.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gtmzvpejo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/ghfqgzygh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/goydctwvw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gxitcjzof.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gmwrqwhxm.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gpnzoxtyt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gaqyeiczg.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gpjiaasma.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/grpghltou.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gyuuwomwq.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gwdbfsaxc.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gzeqoeeve.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gxsjqmiai.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gmhcmujbe.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gfieaxmkf.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gawjhrpwf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gnfwfevpj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gxdhwdtxn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/giwnmmliu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gtpcfuwxf.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gdxtzfjoz.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gspsdrpmv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gnuplvhvf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gnrnnpepf.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gdpxwqncx.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gabbgcgou.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gaijgrvam.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gmvnirvkx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gnodmmnsr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gkcawjdhp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gczccqljs.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gjdpimeki.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gmhbfbnof.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gszcokjpq.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gkhpcpiwr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gqdrrmika.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gqppskjvh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gltvutisr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gmkgwqqcg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gwfihxvbn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/glkuztsdu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gfognvzmk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gmxzvwxjj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gmswsxwwq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gcloamekl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gvhciljhh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gcwzgxgdb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gksagwypl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gwqfpvbnf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/ghmyjxrws.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gdvvfient.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/giiaoucdf.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/geltkzfzr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/grnczjdsq.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gtkzpirrs.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gwwywouhp.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gfudnttoy.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gmohtmluw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/ggsgdnxfs.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gmwnykpts.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/guynoikyp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gubrmimoa.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gzuhsvpln.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmnoczydm.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gormpligq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gjfodrcta.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gnbipjnum.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gawuzqild.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gskjmnetv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gptbtkemy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gwkuzemon.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gumsiiaek.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/geiclkmmg.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gertqwdvz.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gyoywsgyc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/goynqkrho.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gqoykfbjx.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gsfrifzdw.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gadzpsupt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gapvecoji.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gbkzknymx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gmolczgcn.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gqiloroyo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gsxemngsn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/glzebufuy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/grmhavqcl.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gxepnyiud.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gqheakgrk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gtjtatrww.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gagserpzl.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gdgubjast.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gpldeeuyu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gcgnckawe.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gminojpbp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gmppynqsa.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gvrebaveq.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/grbwasvrs.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gogcucsju.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gjktfgwzw.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/grccjbomj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gnptlipbz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/ganzpbfzg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gypmswhav.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gwljkkeht.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/galfsfuun.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gupzdzebo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gygyyuyfu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gxuwkucoq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gnmswjbsu.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gcgjvlhbl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gqyerwogn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gnwqwzehu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gbvwfshlx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/glquwlcbm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gkrgvgrqq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gwdhmmslk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gbdrjjpwq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gmfdnffwm.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gvhqhudfv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gkhniqkux.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gfcwtmjbt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gkgsvzhbi.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gtddwxhju.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gmbwjbadk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gpgmfdqun.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gvvaxlodr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/ggcaetfwu.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gzxfiozev.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gysmaqqmc.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gwlsxwhbq.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/ghvtulsof.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gntlcqxrg.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gdczvhber.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gjnckqtgf.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gdudztoli.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gsivvcvee.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gkuvqguoh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gdjesetfa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gfijikpyj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gisftcqzs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/geegjzyca.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gevaejtjz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/grusnipys.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gfmakisrs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gpivghwsm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/glctphqdd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/glwhpwfpf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/ggmvcmqya.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gcilgtdst.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gazxxsxez.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gafnoctur.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/geduersqe.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gmqejsuvj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/goizkmgem.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gnzydwazj.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/ghsldkzqx.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gozdsioop.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gwflxcwil.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gsfjbgtmg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gbewpfnsa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gfhinotek.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gliwezpen.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gcatwnpil.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/glfsdobel.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gaaektpvu.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gmabgqvud.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gizdriruo.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gqufvujeu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/grnjsllex.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gekelcsmh.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gyuitxcei.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gadghcatk.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gqbxmkxaf.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gwhamuhth.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gdeynixgd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gxfzdwplw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gmpdpnpfg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/ghbtrjimt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/grjjzrpxp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gqegrbner.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gzjcwmloq.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gqdphjwhv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gzsbjhair.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gwiqwjzkt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gmnusurma.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gxizhmumi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gwhbjyknk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gieaklecv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gwzsbmmga.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gwegmshce.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gxzqplgvr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gmwdubcwl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gtxaaxapc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gzaphsmpv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gewifisva.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gwzidyqjt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gfhreedrv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gsxhyjrcy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gvyzxjoam.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gapkcamip.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gioymjwwi.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gbwjnpqkr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gamzloazm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gigxcgtgk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gqsjufwbt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gqfydntyg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/glbelthxf.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/goyiwdvvx.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gszronkkt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/goxyemgsn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gdjxggund.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gvvpvazkx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/ghpawjdqb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gwtcpfmqn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gsksiiypg.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gjpoklekg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gguqhvfcx.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gdozyjhhd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gzdofoaii.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gxwqxefic.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gckvyyteq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gjtavotiz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gqudjyywz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/giggqvhnk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gfyrnjkye.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/glzusjeeb.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/grefcuuku.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/guizkgolm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gyxtpvktn.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gwchyoulv.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/ggdndkfjf.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gpozjjuzs.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gnatlsiaf.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gayouoqnn.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gmlvfuzki.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/geeuwgcpp.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gmxkijosj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gcppmxcql.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gycmcjemk.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gfphubjdx.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/ghzaxypqa.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gsnpwmeod.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gxanoqbsc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gycotaxjs.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gpaogknzr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/ggktrlwzc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gdfvdjruq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gyiwtfdaz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gjkxawook.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gbikihgaz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gnmnoxzau.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gzpvfgpdk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gothbefru.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gkoqqjixe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gimfjrktf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gipemkcxr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gnsfpqwkh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gtdwlosph.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gtzklclqw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gwfkzjeck.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/getcramao.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gcejdiwee.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjdaydmqt.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gobtktmtf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkrroxmhp.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gvjpqvfds.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gxiyobuvc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/ghqlgnquv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gvgoixjzz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gxktnybwv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gurylysqy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gzlpmkmhi.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gdfwefyxv.sHtML


<!-- 参考信息 -->