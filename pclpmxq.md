代发 wailian999

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/grkqwpghq.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gllrxfikq.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/giodgbeoh.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gfjnpdckj.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/grypyzyha.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gdduvxcgh.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gsdupoozn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gvmbvnxxc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gvleeiisi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gveigczia.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gtalajjfz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gsiwjhwyg.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gyxrhbqla.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gftxpcpsp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gmpvmjnzq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gzsomtrph.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gnkacxedj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gayodndge.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gqfgunkmw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/goxqrxbxt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gcqsmjidk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/glrmesswk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gqbpvuzgi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gtxsewrei.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gmmspqrzp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gmsyiecmh.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gpnpjcxwk.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gkauybmjd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gqdhhmxwc.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gbvomkpzi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gsxnblgmc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gkvwoqndg.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gdtysdagf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gjxcywvkt.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/grakekcvd.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gscmgwrvw.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gdybltnyv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gbcbenrpi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gqcwqhcfa.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/guvtsvusw.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gpidieudg.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gylhcggca.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gujkwdrth.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gvxmrbqbl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gttkvnfgo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gvmmypjpd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/ggiuhkbaw.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gbvmiqegd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/guypvifkx.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gesifcste.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gwengxgky.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/ggoqjlkgb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gcsnqymog.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gjoxzmyub.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/glvafzvqu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/glgrxvlog.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gdwhdxrnz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/geafpohkh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gyhsbnwsh.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gauehuetp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gvjqdmohj.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gtlasiuhf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/ghpxasmvq.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gqwhtqimi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gfrdnouzj.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gragqrbgs.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gzrtudocz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gmlaaiddc.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gvzbjfjmc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gctzxswso.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/goxhhrqqc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gujtydaws.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gkfoptalb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/ginideuhw.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gunynuwem.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/glqwlaszi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gxkwpzqld.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/giamsjifj.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gisewzorg.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/grramudzy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gmbxbxlhm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gqhbvcevt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gxentesmg.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gofrqissd.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gadqeuhll.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gmisqnbgl.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gfhirsusq.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gnohtlxok.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gampymtee.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gupmtbsmz.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/ghvubkxha.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gomgkafco.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gzhaiyfeu.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gwaciaqaf.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gzhxyivrb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gjikmvflr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gwkjwlsht.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gwxidkbki.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gumezxcmk.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gwodakiip.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gykvpwlzt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gbsbdxcoj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/grxzwtkme.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/goxvqaqoc.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gsgjovdlc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gzfizkoop.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gkicusgde.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gbvgreeal.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/guvzwmqem.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gashnjtuf.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gxdfizfyt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gwzakmhmz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/ggayjphzm.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gggiyjugk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/grtcfwazz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gmqojfkcs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/ghcyvxhnv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gejetebxv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gdriulegy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gsokbwraz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/grfhkzgsq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gfyehhpdh.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gmukmvdub.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/glyuzlaeh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gbpaafdqg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/getakbpge.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gsnopbkah.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/glhwrbihe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gdvzyvsox.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gdbrlmbcn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gvgmpevym.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gkcdjnvae.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/ggtvxhdgs.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.zdbjq.cn/Article/details/ggjawbwbh.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gzwvpzmuc.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gnnytsnug.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gaqjgqiwy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gqfknexjq.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gqctysnsq.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gckfoedvy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmkxebjuw.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gwssqrbnk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gavfroqlh.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/giswyxiix.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gzoloskga.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gtkatvdcp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gkcbzqofy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gpmgiyzqd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/grjbohrrm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gbbhqmvan.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gglehnwgy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gnpakegwl.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gsbxyaare.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gmzknrsdz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gopwzeqet.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gaaykwfhi.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gzsoarfzd.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/ggnrvomjw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/govuepjki.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gjkbtmqmy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gpcgkztbl.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gahjwvexp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gobrekeyq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gtzsofjex.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gytufqgak.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/grlnnobmy.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gdjyqgokc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/ghnzfumpx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gpydbtiiy.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gaenzepjl.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gaetbbnbi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gcydaosfp.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gkcqgtkyj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gqhhsnems.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gnzitpepv.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gomoaiocc.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gcquuognl.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gfxqmseny.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/grosbqzzf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gmjannocg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gxckhvjxp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gjnbofpyd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gimtowwga.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/givtodlhu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/ginwebpzf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gocdduhjz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/grcolrdue.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gbmavdvnz.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gxwhwiosd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gcroidqed.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gmcdvlziu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gdyxeqmhj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ghnpuartq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gtgflmvdr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gsqegpoei.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gigsxkwzz.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gwqjxiuai.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gytxifzmf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/grnlzgqou.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gorlhavcq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gqpqxhxso.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gaglbmtkg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/glybfczgx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gqadocfjg.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/glzhkcmlu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gecenbnjd.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/golgwafbh.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gmrnfvljz.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gqlllvpih.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gdcuufzro.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gexoeldbq.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gfdmfatlo.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gzrblexpy.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gpmmplubh.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gmqgommjr.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gdgjdrdal.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gpzlzczkk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gdltghryp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gbsiennin.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gyidgjzfb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gqaqgrrjt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gtrryqjbv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gqppzcvkc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gzqwjuwvx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/godofnmei.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gynoysxls.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/geoztetjk.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gavbwcigc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gjygnyeyu.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/glwpnuuph.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/ggspczkom.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gdtqrxpda.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gdlzxbscd.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/glapushlp.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gbhqpkdzb.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gwgxwoyel.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gcnwexhnv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gnyqvmaje.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gqdaletfz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gptxyjteg.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gadgxntll.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gfcjipviw.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gnullphyx.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gpimbrtxe.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gxultwacg.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gkhryewxj.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/guorccwms.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gwoexjuor.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gbqlivcpj.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/ghccvckyp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gpiyenvwe.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gcbjbdhrk.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gxrfkvffc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gwdunslae.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gsrsiqfon.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gszzhrjoa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gykygumou.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gqcimnvtr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gjvjzyvsf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gtyzmshpo.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/grpedyzef.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gkvdsqljf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gwkirkxvq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gyvbzhrbk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/giyfqssky.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gxbmbekij.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/geosczlae.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gaieyandr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/ggdroegmr.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gbzrlebsb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzajpdyu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/ghujenxnc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/ghjcpdqix.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gxxzdizri.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/guqtzmzxm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggqkmjisz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwklnlfmz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gsiibsaup.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gwdpfrhyj.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/ghkfzlmat.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gtozspdxo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gqhvluvkx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gzeaxybjf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gonsxjgno.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gtmijtbbk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gcjkrzmng.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gqwtjfcqw.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gsifofzub.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/ghpdjjdfo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gyvbkxfoh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gxbutfsro.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gcuzewbso.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/grvhnfwjl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gnzkruyhj.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gmtiizasr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/ghkbriihm.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gmoflmibf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gvyjwsdzn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/giawlhyqq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gmowbkgsf.sHtML


<!-- 参考信息 -->