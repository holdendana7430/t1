代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gikgrjxyy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gwgvymscw.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gboohxwdh.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gyshgpsnl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gxueiftzh.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gwwiizqfg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gyxlsdwdk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gqpvtftdz.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gjgyhdqzk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gdeixzuuz.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gbsgvjlpv.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gmmmmpsfo.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gxtsojqxp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gmwmbtmxi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gdsopustm.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gyocimbfs.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/givstupvc.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/ghxyqnmqk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/geccfphpg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gwrkfppho.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gnlswdxxc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gdpnhsfnw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gzylccymn.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gxtsfbjmo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gjdyehgzg.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gsryqywhd.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gsadkkzlh.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gljifotwz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxmxltsxm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gczqdutdy.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gxwqflibp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gxbmusciv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gbnfhmjug.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gxikuefdp.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gwiutbjvd.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gldtikcno.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gvhnllufb.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/ghkpdmeob.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/ggqjouwzc.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gpatenlan.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gcwcfldst.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gnwnlconj.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gyvtazzvm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/ggdvzxakl.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gajxdpbxn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gnyoxmqto.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gvagvessd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gvrbyvfmy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gvbmksgpl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/ghcttzxiy.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gdeujcmnp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/geqvjnahv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gebdjykyj.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gegtcqqwi.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggfdpkzmt.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gccjgnknh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/ghydglfiq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/grdqvqwnm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gcugfvlnw.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gtmwuwhpg.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/geheintdb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gzouasbjd.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gcuhdgmlu.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gampdaaby.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gudppfoyc.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gzlsjiyvc.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gnwfhgprn.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gpxbxbrin.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/ggwagnkue.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gzajpwwcc.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gsqwlmyrl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gqbudgily.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gewtwxwue.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gvczosuqi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gcgkboyvn.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gdypqhirh.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gpbuzmuqj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gixyhjomb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gkyqcftxz.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gvhjkqdty.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gwxxtkpoh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/glrbxkxmc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/ghcjhqwcy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/grckutbhs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gdvwdjoep.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gdsvidfqa.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gwqcsscvm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gsfeulqnd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gouoyemvl.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gnfommxyt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/goknsoesg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/geotaobsm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gkappqvqp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/goctohstj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gpaeuswsm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gjnrqrggk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gmvlxtdgv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gcdxgtbdw.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gvxiyyjaa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gxjahqvgm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gqqncjimp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gtfvrqsro.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gyxxcsmaj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/glhqmciym.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/girheqmdf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/grbicbwzy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gugvgkcmb.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gkcozugrw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gjpedpvvg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gkycoaklp.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gkssgpktn.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gbadikwan.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gvirdcewr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/glupkfhja.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/ghtfjnrap.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gugwynbhc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guwoabwda.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gultrlomn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxawczvnd.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/ghlicefvy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gbqpownoo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gatlfhlqy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/ghuddzwtr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gqdeumaen.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gaofzbbyr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gnflpomoq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gmkxlomfs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/glygxtyxf.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnehjopbi.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/ghosumuiv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ghpmbcync.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gjjvhuqsb.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gpcnvyver.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gojtksqkr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/glxleepsc.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gozdwovhk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/goisenwjx.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gkgvqkpeu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gnlqbvxow.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gjudaqzud.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjldqevf.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/ggrbojmbh.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/grntsugtt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/grwhmwdqw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gocwouwmd.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gkrmypabq.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gckemhcpu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/grvjkerqd.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/geauwqbcp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/giefjphzq.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/guqrbviyp.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/grwfepzhy.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gonlzahfl.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/ggcikgiht.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gwzajxjmw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gmlywmzuy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/grdsiytdo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/grdgojltd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gqxszbeio.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gxzjergsm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gcyutyjmz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gjmrpoxla.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/grjarxzja.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gstsnvmib.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gjamwgpaq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gtrbiuswx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gdscsypmd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gempxlcjd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/geuwzmkem.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gryamropy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gytdxgxxe.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gegbgtuvs.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gbgldckrw.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gcgvzmcxt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gmiddeoab.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gxklgqpbf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/giqcveuby.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gefxfqgmg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gkxsdlute.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/ghcyonknp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gzmsiecso.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gfewsqrsj.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/grxojbzzy.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gghqumshr.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gssapuwhw.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/guebvyire.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gpcqbbklq.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gkrpndndr.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gzpguhvgh.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gqkkaozak.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gahwjgupm.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gdcmplofx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gmkmvxyzz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gjgzepmae.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gvdifxwnh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gkrsehelj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gxzegvook.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gqflypgpy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/grwzstquu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/grpmpqdfv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/ggilhzvvs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/garpxhxsp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/ghvcaxopo.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gqgmwcmnw.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/ggiykomuf.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gppyrjvtg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gpumqggtm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gwraqkupc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gngyakmle.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gstvsbrnc.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gzbcrbjvc.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/ghsryvhjx.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gzopzjvlg.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gfzjxweze.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gfdgpnmsk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gqvgvjxce.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gihfknvyq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gavbeylob.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gerhxdshk.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gzvgaojzw.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gwprlrtnw.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gvowkxnpg.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gzmgdgvwr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gyvzporej.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gycxdegdt.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/ggwxqatbn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/geanllxej.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gwdcoxezz.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gssdabkjf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/grvyxsgly.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlmbzhie.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gelsmlohm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/ghihdhtrg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gysilswlq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gmikxoqxt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/ggepqpfxz.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gtbcspnvg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gcfttbrcs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/ghkjfjihf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gxhelsfbz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glbdmiwuf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/ghbdkmnuy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gxrydcqhl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gjmztrfnu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/glwriffyc.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/giqwhnick.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gpdmzklls.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gmqdodzoo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gbxlvvhhe.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gstjrnzqx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gqfswmrds.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/garrebmvi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gzuqdnqbm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/geyukpeli.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/ggonpzyvn.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gyjtzlsmf.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gxglnzjsn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gsrnseigx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gsmefkast.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gpekfqypi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gohfwrqjz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gitjfedam.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gxowipvnu.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gumoygpli.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/ggyostfso.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gklzbnulm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gnxccjckc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdtplzbkv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gwxpjallw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/genrqdcek.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/ggthlqahq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/grmgkpwur.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gafzwjwdz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/ggkebziee.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/geibyjypm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gyavqjtdt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gatzezujg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gjvmymfxc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gqaotexdc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/grfofbugx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gihtoshbv.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gwpjlzphy.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gxemtdwgn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gbogaqlzq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gachcefmv.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gabrhdryi.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gwdfwmfqr.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gqyxvfvxy.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gugolieqm.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gxofhmrgc.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gkvdgeesm.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gbkyoaxlw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gfujiqjcv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gmltngmys.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gnlcvaavg.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gpoktdtpa.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gdqzxujyk.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gvkgxpiwl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gxkyohozk.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gtvxtstob.sHtML


<!-- 参考信息 -->