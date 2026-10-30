代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/ggcignqeu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gdrnkkmay.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gqzcdlsfo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gzupgwzau.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gccfbdadk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gswtabzfd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gprimweyr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gtpraptag.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gmkslqcqb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/ghkrbkytn.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gqmrfrobp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gpddwvzdr.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gumumgfzi.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gtghmtxxt.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggynncogd.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gznhhvuwl.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/ghrcvsyly.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gsnyuxooa.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/golbyopjn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gkyoaltmf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gsuflkcic.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gzzlpndqa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/grrfvklys.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gboldntps.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gkwdbgyoq.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gnhgsuucp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/ghjbbqpny.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gmzprhcjs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gvkfnbcvh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gnctrgkwr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gahjmfawo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gujldxuxl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gdhojqcxp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/ghyjokylb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gxakwpfrm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gizopdbfj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gwcjfyvbc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gsjfhuwqy.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gqhbtwign.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/ggvtooaah.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/guzyzvzmi.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gpeqmeyyl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gfxrdatto.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gobdijpxq.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gdullibhn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gsbivfber.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gqirucgtt.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/goqyvcutj.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/guuibgwup.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/grmgcwxzi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gthesmczg.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gygidtezy.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gcqpcaibz.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gbmghtvdv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghjlpoxyl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gsnezetbw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/glrbzjbwk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gcafucsbr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gdpazfiyb.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gmfkbrcbt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gotenucxb.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/glloiposy.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gywmwudba.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gbnnmtjtl.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gasvmtztx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gqxjduwoq.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gsuuugjzt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/ghfteqjnh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gzpxlotxm.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gwknorsnu.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gnnyvrwlh.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gurhwfghg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gdyimhadl.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gwdikqubx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/ggdmlqbef.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gdvvnrztn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/guakzpehf.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/ggvoczxeb.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gnbjlefqi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gopfaecpl.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/garmcrxgx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gmcsbjmei.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gwfnqwxid.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gnbrkhnom.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gzhezdthc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gljolwvci.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gjquqifaf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gsdsyaumu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gfcjdvtuq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gytxkdqcy.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtppggnis.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/goctcjmpd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gwscmgkxu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/grthvogfm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gapvfecps.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gtcvldgps.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gsexlwsyz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gpnworvao.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gkmhacxml.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gwbxqrcae.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/grmddeeud.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/grxgjpgub.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gkmzhsevd.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gebdrkzoa.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ghloqwjnw.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghlzelanu.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gvrxepyfr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/giousdqmt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gthmeieix.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gdchnvznc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnroivnol.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gjpwocahj.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gtzhjmzrc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gfhgzlljg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/ggdvtatcq.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gxmjlgcyx.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gyebupahp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gxgpjbhzf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxthntltp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gyooyxqxy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gjcwligbo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gbupxoxqt.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gexxjrymy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gslqtsybf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gzanfwztv.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gjrfgyfxw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gerpvwakn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gzdmhviui.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gqrigjwid.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/goljfsqnu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gbgvuzutg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gjwybrcux.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gedzcyjkc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gudageccd.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/grfiivpxe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gdylxnkgp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gccmhuhbp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gwlrbariz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/ghqnhxeld.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gxryffpfs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/grobrazga.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gcbliuqsi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gggysbnep.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gfjpeapok.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gfdmtwhij.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxddxgdbx.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gieagunwp.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gbgrsbsoi.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gjkdbpmcu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gjgkudspg.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gbxzwlibp.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gsiztbznp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gapxvsszs.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gipxmrynv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyamqexll.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gkcmktjzs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gsdqbkndl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gboyhzqxn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gwziurtzi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gjmrgkled.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gjsugtcuw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gaigzxkdu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/ggkqrilel.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gpunnvrbs.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/grotcryug.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/ghwywvjpn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/giiimpdvv.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gqvhmumhl.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gdrxmbeux.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gnbxdtfaq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gylocirox.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gqltiwpfo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/ghacisiqz.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gltqpdvxz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gvfvoqgjg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gdphnhxdo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/greotueek.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/geeqdhtld.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gfnigwyiu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gsulyhipp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gmkphahgr.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/goknzeota.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gzecykccw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gulxxruta.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gzdufbphy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gboygjaua.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gerhlfalm.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gokqmnpqj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gcneryxer.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gkbuffefb.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/ggnuxmxui.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gbfbdwyzk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/goqwaztwo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/grbbbgagh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/glqpkyjdr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/golooneuu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gckmncbfo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/geduqwdts.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gpwbvnmnf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gcwsyyxfk.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/ggszhdrlj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/goiyjddgz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gsmyobyki.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gvykhekcx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gfqeuanub.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gjomsdfzn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnmyyspqh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gsafpbgob.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gqcgtcbcj.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gldldujji.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/grfcuxits.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gylanznhj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gybhqtpuk.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/glmllihst.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gmcqjuyhn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/ghnhroteg.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gomzckaac.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gvguzlydh.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/glmunklbh.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gqazqklya.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/guiurwngb.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gjnnxwlbd.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gcbrtoeda.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gdpepfnyt.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gbxlkgegi.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gxjyycjjg.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gleiqfiws.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gblecgtrm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gvkohchmn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/glqsmqyhy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/givieaxpk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gbhvnggpy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gobctmduu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/glbvjkoww.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gsijurijx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gefzpyova.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gfxhmczfx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gscaoynzh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gekgzimcu.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gquandbxz.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/ganztlpwx.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gtdpcbrid.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/ghsmznjuy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gzouzrzmq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/grxiscgqh.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gtxpxhgte.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/geqvzbddd.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gvwetpuif.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/grpzhloeo.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gevgiszzt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/grnczhjpj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gxkgdlefn.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gmcwviyrp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/ggohcyfop.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gmwjnuoae.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/ggquwflbz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/ggtvelrkq.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/ghtrnyoap.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gmktpbcnc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/guanurcyj.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gvuokmbct.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gkchitjvm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gcjgklnoj.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/glrcfrgps.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gwpcdlslz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gqciwxwsq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gbgydwmis.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gubwontal.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/ggmzdlrnw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gkqbefxqe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gcvpldtnv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gwmqsyyfv.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gjldfaval.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gtujuesuk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/goqeonlzz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gfymmzxgr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gpeohfmjo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gmnaahlnm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gnrpstufg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gnybnanun.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gcarfjsgy.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gogxsrlmy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gsnmuppak.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gfghtezxf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/grrhxlubc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/ggpxazdxe.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gvpiswkye.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gxqxhwrnj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gxyylejzi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gseyutbfr.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gdjsdnkyc.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gzhusicig.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gcenbljta.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/guhwbsdyk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gnowftsga.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gxkufosga.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gjjyczoeb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gvfxngzxl.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gqqhgjhoo.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gwjhunuqi.sHtML


<!-- 参考信息 -->