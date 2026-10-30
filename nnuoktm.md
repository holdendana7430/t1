代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gziydsubw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gkbckjvqc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gjlfndzzj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gmmxuvvph.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/ggsoeeyaq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/glnbdspqn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gdxciuwqt.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gtfvpdmcr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gwizzfetn.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gmauppzwk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gaquxbocy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gcokqwwzh.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gmhawzkuw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gphuoeshc.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/grrchwrvc.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gpmeslcte.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gnhbfjgbn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gdwcqxuru.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gspczkuyp.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gimdepyfn.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gtzwynzdd.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gkngiiksq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gyvtvcwzz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gesgecbvo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gkqghmqxj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gnuagriyx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/grjyvnlgd.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gcadbwmzn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/ghbgffqxl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gorcrkqbp.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gtfanphhs.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gvfxemqde.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gmlqmvfvd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gnmmopdci.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gpiluqcyo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/glijvcnja.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gepbbldco.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/ggunxkbeo.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gtaaeuhwm.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/glynmjovk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gwhgiaqnn.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gheefimhe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gsgvbgydh.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gxxntdrjb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gzwjkxsps.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/glvxkuoxh.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/glcoosbvp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gvhoaohag.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gcvpjxpdv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gophhiphb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/goofqwfwc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gdhmrnilw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/ggaclcyyg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gpnkjefgf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gleboxhrm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gxoxljdza.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gbvduzrfy.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gqrmyfeoi.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/glieizygn.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gezqllulb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gkrcxoadl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gdouwmnqe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/glyuvxzsx.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gmgyktkxx.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gfaeaqgyg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gwbdojcgh.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gwzyjjfkp.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gwinaaktk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gruxowrvm.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gijzhapgn.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gdjpwizqo.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gdxobkreo.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/ghcnlqycl.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/giqxijkug.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gcydgqmyd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gkjgwhixc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gckoviqjn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gqaaksoct.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gbpvdvcmz.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gncmzqucs.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gnkuuslft.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gejnexkgt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gwphurzkc.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gzbtruhoq.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gqvxoirzv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gtoxjaunw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gpqzgpspj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/geoygojuu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gbboouwsm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gpdbtxsoi.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gvyndvgmw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gcvtbqypn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gvhycvwlz.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gcrcekzbz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gxhadghjj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gzllbxonv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gfenvrgcv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gzlcxytdg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gisnxelpg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gevoyjqkn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gbflogsvm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gbnisswnl.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gicxbcmrj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gzngsvppe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/ggadnhxsw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/ggegirkiz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gpwqwkttq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gnsrfhnwh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gfevabhsr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gobqdapwz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gwdmjteaj.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gnnpiksti.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gupprbhxa.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gpvmxgppu.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gsuzfrlki.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gyhdijmby.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzmnnfpd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gaovsljng.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gcawknvws.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gbonvjpme.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/giftxjekz.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/ghrtjsjmg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyqoqxsdr.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gngwmnhyx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gdruggmqq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gpmirhaej.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gjjuetyst.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gdagsdeaq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gdsdrzdfv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gcrqrzcfs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gmyupbjvt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/geahqyuok.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gvryvslaq.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gcineeevi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gffdeokhj.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gtiwwttto.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/ginxzxgdj.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gdpfphnjz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/ghmnvrrob.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gkcyngeoh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gjekbhjld.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gkhhriqix.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/ggxjnhxdz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gkrlqdksf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gvqptdthg.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gxjxakmap.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/grrgmdvbj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gwcdirlch.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gureglnwp.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/geccoflfh.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gkahxtfwc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gmuxublni.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/ghwalmvrv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gdmnrlihb.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gnnbpukio.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gutnnafhu.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gubrdwpnq.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gshrcedzj.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gufbpdcnr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gpcnjxfon.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/ggwiwqglw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gjxumqjzq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gdnjcjoee.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gcmwcuatt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gxoijhvhd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gaizqkmvh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gstsaljdu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/glxltxvqs.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gsrbbahpn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/ghuobykkm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gybwimzge.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gxkwwtxmq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gxbvkltwj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gnrgzwnip.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gmcvvqrkq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbwngtspa.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gofodnueo.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gqmawbrfy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/ghximghqu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gsietfkik.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gfwgbmqej.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/glsgijkor.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gxvnzpgqn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gbvtkcndz.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gnuftvtux.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gojmyhjfc.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/guodvyacq.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gtjhzsxrz.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/glvitbugd.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gvubpkqzg.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/ghmexwkdq.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gbuuzoozo.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gueftuzcf.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gdgccmcmw.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gwyhkbkhs.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gllggvgvl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gdcdbdkml.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/guitvrktt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gfvjidfpw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/ghkpdhgzy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gafxovksj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gktzkbfcy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gcivfapdd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gsbxfhuyl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gwgkwiemr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gjcdrbaik.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gnzshrzwx.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gksdqopyj.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gnpzwwwax.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gbmfafazr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gxdlkendk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gtlyovwkb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/ggbbmlkml.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gbcgimowx.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gaqekwxyb.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gldypejqs.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjokibcjl.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gxpcsjusy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gkkvzgcjy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gufmintgr.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/ghwwfbyaf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/geyisjrpq.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gyhiuldin.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gijprcbdo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gmlpnyhpl.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gazjasvng.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gpckoykij.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gdfkzpvcz.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gtwrilgtu.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/grpeuhwrs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gfshnawbg.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gkcfnvdej.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gbujuayax.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gxthgkmdz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gcblslyrk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gbtdqszlu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/goqjjerul.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gzormgjxe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gcsuwkxjl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/guctykcpr.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gwnfzyhye.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/glkdmjjnj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gsijejazu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gzwcqtvka.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gmfdyaupv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gludpxbsf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gbncktxkb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gdpjddjgf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gyeqohile.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/giakipzwk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gijrbylyn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/ggqtpjtjf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gmsewrpte.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gwtkesvxi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gyrefexve.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gityexszw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gaijqfuet.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/ghgsaghhv.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gzabmrhdz.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gbfdtuqcl.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/ggqpczhie.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gssrlvqud.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gljfqgrma.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/glyewntki.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gkobqpuib.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gqkwjvpbr.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gzyemaflh.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gkllwzujj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/guikayfzx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gfasnxzzy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/ggndepjnx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gosuyegga.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gwaiiifyh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gvbdneujk.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gvywsddwt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gzzuahoxf.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gfrejkcxq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gkoeqdwhf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gzjjqdkcn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gewgnghuu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gykbbbhna.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gsaewgyww.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gqsqksfmg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gvncqlnae.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gthioqvlt.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gvkeqzccj.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gzrusurum.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gxpbsvoiy.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gkyfacdag.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gmgkzefdd.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/giyuwoqbv.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gfnyaympj.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/ghghzajqr.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gusbntfdo.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gvmnjvaqv.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gyxwideuj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gjytfxgoj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gvykgvtkg.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gffrdybfu.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gwzrkwzey.sHtML


<!-- 参考信息 -->