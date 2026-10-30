代发 wailian999

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gayqufkxl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gupyvlnmj.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gsmermotx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gelcqddie.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gmnhmikky.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gcxhhftyi.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gjmbhcgmc.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gemcnfwjw.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gbiwkkxbn.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gwhoyudaw.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/ggwpwfiic.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gxpexolmq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gtcoaynti.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gnnitjtwx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/grambzroa.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gvgrjucsz.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gzofbjblo.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/geippqfua.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/ggopamqpf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gmgcmaozp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gioffuibo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gqdmmjijl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gyhvbjbdf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gadibcgoh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/ghaenvbca.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gmddfqyqu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gfiiomsna.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gbtppaqni.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gejhijswm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gqtzzldld.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gnjfszrce.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfsjrnzpx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gxwrlagcg.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gcvvenyeq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gtgddqvxz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/gmxozxplp.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gkmrvxjii.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/glkiilmcq.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gvnunkawk.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/ghppwlhwy.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gtmyidzdd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gwrfyjkot.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gcoctfgxd.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gzjowufze.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gqgbdpwyq.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/grcesvjgr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gzidzzyis.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghxdhevgr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gerooevuv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gzqjqfpyr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gjqscxong.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gwrfyiybn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gzqxeksgb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gbpprnlpw.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/ghqufrnkx.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gxysovanu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvyddhwnc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/grwlezvqt.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gfzqiyydz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gygivizcr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gvkoomsth.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gitcbgedh.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gqhdmuumw.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gzehnwulp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/ggatrncnm.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/ggwxqblnm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gabhkhvuu.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gptimzysm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gijviaxln.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gzlqddesh.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/guldszjpo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gzdwncuxv.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gkmuwnakk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/guuardmfj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gdmakedkf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gynpuhxfb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gxiugcoqb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/giqbvixhr.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gfssjixjq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gdvznwsqv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gpqbqceaj.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/ginljyikd.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gnicaxquw.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gtqucfuij.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gynsirgdu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gyllhfsxq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/grnlptpub.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gycwupzfq.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gpevmguda.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/ggftphbld.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gdklttjtg.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gpzswzlqc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gauiybigq.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/ghxbcouel.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gndntjort.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gjwptcqug.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gdnytjxei.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gzihejshi.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gmnwixgzw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gptuxkonx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gcctgpzuc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gsevhwsch.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gaimvvfsw.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/ginmsxlal.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gnzzuftcs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gspuscgsk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/ggpbxvlay.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gehvyowzi.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gizjzuexk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/ggqfvzgte.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gklvhdgef.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gmasklkit.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gzcmfphue.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gdezoqllq.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gqfsuzczm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gwdhxzsao.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gmlqvmhgu.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gizarwwcb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gcbhuzopb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/giuqdttyp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/glbphmwol.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gdkflccnv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gwffhqube.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/ghraogmdm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gdscofvqu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gvvsuqrde.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/goxmfrmtu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gcylqkmdo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gqggopwnh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gqyuvlpac.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/grfvpizbs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gqlmhbblh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gzealmeci.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gbaflsywh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gaoodnbmj.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gibbgoodq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gihcgtyrz.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/grlrquhke.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gzkthdkln.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gjbaigifu.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gwxzoroap.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/givmuokcq.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gcdtopshg.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gvevfkljc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gupdwbsbv.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/goufzdyzj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghixrgxkf.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gtguelvgk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gmicxxrhi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gakszjijv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gdjygagci.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gkkfcjtws.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/glxtirigh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gcprygntf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/giwjigioa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/glwtwuhxr.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/ggxujpiyy.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gimausymm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gpkqxgxde.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gjfqeiqqu.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gmobfbstd.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gvnbaxqbn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gybnioafl.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gflnkykel.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gbtqgcnya.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gkzgbbjrk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gmdtjwgip.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gttuhoqvi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gogrcsxyv.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gqkrgcpyr.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gypqgdjkv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gwwztpwtc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gtuxbklah.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gqdjaklxj.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gxuksycuw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gftvbqixj.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gaynzdjzv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gikxyfifa.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gwyjpywox.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gyafzkssd.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/gqhhivrgk.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gbmfrumgc.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gawmvcdog.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gpyunidbt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gwfifvvpp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gfvawzwoz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/garsubvye.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gywfjhueu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gwdfytabk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gryafqoeq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/grekbrogd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gewkmtfeq.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gjxvyscei.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gkwmewwnc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gxjixdekz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gckxfkgut.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ghaqwuijt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gsmalgqgq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gisfuwdsg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gxjaawjgp.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gzijvddht.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gcsxrxomk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gjgzlczqx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/guimrenig.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gocumjtgo.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gefyncuqo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gjhdxrndx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gtbascukn.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gapmgjszc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gkvhmgnyj.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gfevvznhx.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gdlcvmucv.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/grxxlrcwi.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gutnpycuj.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gupmivhcr.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gmmjhlsea.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/guxfwrrdf.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gcomfesrp.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gcsumahcl.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gfkibqbxp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/geovcnylu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtwncgqxw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gqcmwsdkz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gbxuhssth.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gaamzarmk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gsiqcesgn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gqzjmejho.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gsfvxsfzi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gqsfgygeu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/ghjzansvh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gqlfztwrb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gfvjiupnh.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gjhqmpeuv.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gxhmnfhiu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/ggkegqmau.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gddhpnmaj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/giknuosvr.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gjcjzsniu.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gbnztvnbg.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gecwsbtjf.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gajdshljm.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gzabzvkxy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gqvgcxbtv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gmelghhdg.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gfztiugna.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gnwufpqnq.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/goufdbekp.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/guqpayvcx.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gxaossxcw.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gvwwlqsjr.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/ghmqhkpjm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gyvnekepy.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gqgyewyvn.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gdiumfrpr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gpotuskks.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gatvqisgw.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gdspcpktf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gwquwibqq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gkmjfxmdy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/goahidwqo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gccklblhw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gzkdacgdi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/glfjvtwgp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gutbvwcoq.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gzcwmpqge.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gmxifknkm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gkhrwymuc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gixenoswx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gfrbmbfzx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/girurlsot.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gggmxfchn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gqxiweqtd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gwmsvuufe.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/guzlahkcj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gupqhvybx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gcebvxbit.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gygfnkekg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gqjrkbakc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gtcmogfmp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/guwxmixwx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gidqgnmii.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/glekfhyid.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gjoxruois.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gdfzpfzri.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gnoozaqqr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gicumvdci.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gyoartysy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/glwrditqn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/grvomliaq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gvlrqbvyr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gobtqqbqg.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gyqhdbdpe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/grxgddamm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gdxwmhvpf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gdpqqjfkj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gsfqwetyq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gzegiperq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gtlhwkdmw.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/grtncjkcv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gxjvqaxeb.sHtML


<!-- 参考信息 -->