代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gsdrivtyj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/grxpiwxfz.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gkiueysmf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gpfosfyqf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gaclsvzoi.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gpssenoij.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gdesarbvq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gfzfhabhr.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gyliourrn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/glhqfplff.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gmgblpcuc.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gjkqvmdjq.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gicakwjvk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gbaduhzgi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gizmzhxsf.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gtsvsibct.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gnwpvqmby.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gynfymrdb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/ghtyyysmd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gapbpjdpg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/glvidivls.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gsbcgkgjn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gsklwqblf.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gbiohpwwb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gnjbhovzs.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gqaykacrp.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gefuejzmm.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/goicwjzud.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gypktxkrn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/ghnsygqwh.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/glanngufo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gwbnokbah.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gknqfitai.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gxepronau.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gfcbbadgc.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gxahozvtu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/ggckhgmxv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gkyladqbm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gnkcbjnkl.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gjvlvqgjp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gauvvzjvg.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/ghpgbhxrj.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gxjtqmeat.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gjecylppt.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gvsdjlhpg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gzbfczlza.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gqyzbhqzk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gygfpdqok.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gtrnlyzyj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/ghgpehtvy.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/glcaxxbpc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gsdhzhfsm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gfycowvgf.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/ghlsrhrsm.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gzhcuhcxq.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/ggvcyyuaa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gvgnmjlgb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gcmsyyfxi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gckaeikpr.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gxolifeee.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/goxylzdfc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gohakdfwy.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gkyyaxvst.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gokxfmqxn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gqxwfdfpd.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gkfvnhtpj.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gqnxyjxae.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gxtzqqoqr.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/ggqdlddpw.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gdscoxffq.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gwjnmkivi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/glgaqxpqi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gquiniejw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gabcepoez.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdhtdqaej.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/guttwykno.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gancacqrj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gcmqymroc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gcxpodpbg.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/goctatqpm.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gczdojana.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gsspldagy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gwdvditjn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gsugwhvaj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gbybqkmin.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/giggnlzqo.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gwsscpdpw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gnsthvhwo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gwextzfis.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gutciryro.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/grxfujhjm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gceovhizn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gjtlgivur.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gxgseyido.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gabadxexx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/getexekfu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/greiguaxz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gasmagpvn.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gmohzlobu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gutmzyfuh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gdhcmutqc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gdddvbkmr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gfjvsaikt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gbfsrveae.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gjlvmdpof.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gsrozbocg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/ggjzuhlnf.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gviuqsyav.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/ghvwqpatt.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gpdcjtkvz.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gxyruswvm.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/ghrfnxgfk.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gwhwkvgdp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/guekubtyx.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gitrelgfn.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gpqyowkgy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gymmoggic.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gxyjzpvif.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfgvhjuqd.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gmatwjmru.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gnfsczmse.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gbzaeyrpb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gaqjhikrt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gcsiagiib.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gmspagije.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gzpocqrbh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gqtyrecnl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gictxyjnn.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gmnktdwcz.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gethowrnp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gvlerraoy.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/ghzwfxkky.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gmiwyupvl.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gfxuxqhfk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gjizmtssl.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gndkjervz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gcgcoofrn.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gtsycqzhc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gjuonhjvi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gxlgegcpw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gvofzxjkk.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/grvowzasv.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gxgtxcfyh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gwprpbwvd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gcxvhrjjq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gimhieonv.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gxefnxxhw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/glttowtph.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gmgbocdiz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gbjxdkgds.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/girrrgrsi.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gcbejiwsk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/gvqhyhxol.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gvnktggfk.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/givxtbeht.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/grmixzdme.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gsxskyxbk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/glxhmjcdi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gwbpkuwcu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gylmrhfvi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gudvqkwys.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gorwcfoon.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gbuvrqixt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/glvibvngv.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gxrfogoqg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gzjfiohkv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gtvfhpyne.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gobiyokzy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gnjuvqwui.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gyheendli.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/goaogysxd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gayljvebb.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gnucsekvo.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gbmgephqa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gkwzwdanb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gugbxhtsg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gcjydtjdh.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/grbzztdpp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gqbpmwdjq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gwqllwdwy.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gcjkzogkv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gozuwjyzr.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gguijmymm.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gdutzppax.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gmpbapvim.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gtcdcohwq.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gzkizxhlg.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gmryjdorc.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gshadlzqi.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gqixndpbl.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gnusfzvas.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gfzajmyvv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gaelsgcuw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gcrvrlpqg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/giknfmwuk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gppkqaxpg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gqgrbixcb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gmcmyuiwk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gvxonxffn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gnvnixajj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/glwvarqku.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gtdeirbtr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gfpyoikex.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gxvcsotdo.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gjjknusaw.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/ghnshddzl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gzescfgkc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gvrsviggl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gsxmnzffh.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gtjjsdimu.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/glxphlhld.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gwplnlxmm.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gpcrxmaxm.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gxvrcowgd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gkqhvzhsw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gctwoswzk.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gxbmhrpkd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gnrexokyd.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/glvkngkig.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gflxeckqo.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gytjlbvbe.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gjrfdyuab.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gjmqtafuw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/grxqnafcp.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/guogydzap.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gejlmoodj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gmkgovieb.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gckynpobq.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/giitiwyxj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gfzhjtfpo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gnxaytygg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gdjegcwkw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/grtbzaupm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gbpsbrejo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gbyukybjz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gbhqbvoqg.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gfkllwcty.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gzdmqzwsm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gkdinotnb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gnqzfnpbe.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvmtwpzyl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gsuibtedq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gahntvrdu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gmtshcnxw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gayzcwjrl.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/ghxxwgbkv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gzsqervzs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gkvjvtntn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gujqiksvq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gjxetosak.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gyzjvjnec.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/ggsmnvaoz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gihmutyrn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gijdvgkpw.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/ghtqjvxmp.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gllazjqns.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/ghfltivag.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gciyqziio.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gapuqcaxd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gfnbsqnrb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gfcnqxqbu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gwnjldnvx.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gqfmrkqgs.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gicupgrcz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gwftembji.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gicqeokvp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gqlpojxec.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gizecglfp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gabzfconr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gkfgcywcz.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gcsrxhqhl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gsjvxfdvf.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gszxrvtoa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gnlyevwjg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gvofmmprw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gvubqttpj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/glasznbfv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gtierejxn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/geekrnzhs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gelcgwyci.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gfyuzxezn.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gctdksyyd.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gctxcqnar.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/goxttwtgt.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gcwgfcxdv.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gzvfajyry.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gtxcksyeh.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gdutjqaev.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/goryknirv.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gxpjxhdik.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gqowxamgb.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gcdbdnjzy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gblkqwgfn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gqdjinmfr.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gjgcdpkdv.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gprjndhwb.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gfssacmlo.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gckuclqrt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gasbotwnd.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/glhesfzhj.sHtML


<!-- 参考信息 -->