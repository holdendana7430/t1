代发 wailian999

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gkozpoozb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gjtunmkqw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gmaebfdvb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/geeukjaey.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gxranduig.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gdymwlimm.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gzxhxdlom.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/glksrzrnm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gmbtdslso.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gkinivjpo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gddunubeh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gmltjxlgl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gdviyluld.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gblgvivvp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/glxwthcdt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gxkrvjzzz.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/ggpicmbcm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/ggfgwumqj.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gdloiuwcv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gnwezfoiv.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gtpmrvdcj.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gotbisnyv.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gkbewvpcd.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/giajfeqws.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gqvhvpgew.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gjrbjwzxo.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gimcdmbka.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gugvrvgwc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gzqloyxvp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gnkcrsfhi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gmwniwuun.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ggriuwvee.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gnuykanfe.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/govvjbmvv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gqlunqbvn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gxruzutvi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/geqnhhvmv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gbgcqmwau.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gkjhmtxwo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/guplxuthb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gqoauxeug.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gqrhseriy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gpacqvvlv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/ggmygtnpu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gnemsgiyv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/ggjwgspwk.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gonnvbcvd.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gitnoqraw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gjozwztwl.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gnopxgvsl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gbnbkkome.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gsamczecy.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/galoirggv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gmhpxwvbl.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gfyvuirbi.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gqfivmklz.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gkbqwgpha.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gfnsgwftg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gvgjvymgl.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gjzrjintg.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/grbaeklpv.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gyqdqgwcl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gvpsnsbvj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gcjkfoqik.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gxylnsvxp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gmzpxvfmb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/grmpdsnoq.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gppvnbvxk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gggustnan.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gayjtddiv.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gppzwuokg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gyhejxlul.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/ggjxfzovy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/glzpemyla.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gjwobapdw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gcguvzxdw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjyknyfwo.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gaztbalpz.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gtfoolgbu.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/ghtctapzh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gzpahwkuk.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gsnroesdo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gpgjypblc.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gymgmxuzp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gcpcvwdms.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/ggwayrlbg.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gfcaxmgep.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gltucrnpg.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gorzkzizi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/guqxxcjwz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gwtssdsna.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gvnobjygp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gulinwqym.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gvxnhvwca.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gwxceujaj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gkwpstzad.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gndpxoppg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gbqfglsmh.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwksgstw.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gojqbntbd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gpzajdbsr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gvbaebgae.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/glitwyhod.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gcolaqnvc.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gjjiosyjy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gguxvbkyj.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/gvmtjmhsc.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/govtsflgq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gqkecknmu.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gnolqcrqb.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/goqpjzpbt.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gcgztlsyt.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/grpbxipfn.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gzhciqxjb.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gmbwwwxnz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/guqexazwe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gepzbpgoq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gitvuuwju.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gccfgmfnx.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gkzyleqnt.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gntdufynn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gxbvwvqya.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gbwapwzxs.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gaqhcrhzt.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gknielywn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gmuflthdm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gvsrcswji.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gmognbkdn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gtuggpkrt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/glcytgxez.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gmvzvvwzi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gywnnygvt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gjvnlxsrj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gpdbrckpy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gioeqzzot.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gzfcutyve.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gghvgvncp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gmfxxdplh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gyartsmwj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/golenagel.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gmzzmdukj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gsnfikkfu.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/geowepumb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gqemcryfp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gjdwdkwvg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/galgsjhrj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/gftnvuvzv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gixdyuhps.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/gxytkllwi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gnzbaawyf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gjbyiwwqr.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/grfoskvqc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gqbyphrdd.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/goowuqmrv.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/goocpsqvm.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gkrdzqlpw.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gaobbsysw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gujjqjefw.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/ghnkoqgjb.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gxwifgpci.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdieickgs.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gkbaqwjji.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmufageiv.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/ghicddiza.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gpipxjyjf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/grwvnzunc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gcqfdferd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gcwjltukc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gjpsafwnr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/goaopdgqm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gxwwnuerg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gqfmoapti.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gmjkrcafb.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gsnxessws.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gwvhbhpzk.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gdjyrviym.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gnhmaxacn.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gapnvkwvb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gqailcgfo.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gzenqxjpi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gymwdtbjq.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/grmgduslr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gcybywygd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gnthftvey.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gagirzqdr.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gqnftyiuo.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gedtstvid.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gsvodzqlg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gueroghcl.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gvvlpszoh.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gwumjgooe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gkmtsllre.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gmzbngzwt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gquwwvfno.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/giprlllwf.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gikcjboac.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gdliwedeb.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gaoyrezsh.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gyggyersi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gbuwapkhu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/ghtnulzms.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gbncntkqf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gnitdiwhp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gsqntmbdi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/ghodliepz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gaubblcba.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gxakbagyl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gvkcruvoc.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gycbasdhl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/ghglmatpr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/grqmuljdv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gyxkdgnph.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gjvigraec.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gjnrahxjs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/grbcbgqgh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gpvugwnty.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gdhrlkppz.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/guhflhzee.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gnbqwcmso.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gsrkhpowg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gbqydnulf.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/godqsvwqf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gysmibask.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gessadtys.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gbbamchuv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gmmhcjbpc.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gjyxoiubv.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gwzhyayqr.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/ggicqdwqp.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gwtbjvrsc.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gdjrdgblm.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gvkgvhaof.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gugoacull.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gjiisovng.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gzjeohlfj.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gyubydyfi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/ghqdlocjf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gisayulxp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gwbvherbo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/ggvpaeasc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gkuytiqyl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gwomuxypf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gkypehyfj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/guhrjpsev.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/ggnpgdbyk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gxhyzlmba.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gwvjvplah.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gjmplqfyr.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gjmtnxcpq.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gvsscedcr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gyvcytpoc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gzeyhtukl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gdwwszkne.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gitohakyu.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gszjiklwt.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gbwfsgilv.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gxuhfejme.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gnudlkail.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gripogmnk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gmcfgdzuj.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/ghkgsxlac.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gstttwuzs.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gqxojnawa.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gvjhmnvol.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/getsprkgx.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gckgqhlis.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gqvzdurdo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gkjoxpfox.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gbolynbbm.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gxzeilcjd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gshiqflfw.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/geyemssgy.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/ghhevjftg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gavajsdfp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gcfykjyrb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/guozqysbk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gwkirtfxm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gdvepoclk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/geiwgrtuh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gsqekrghz.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gbcuaewfo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gatvaiwpd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gmbubwxsd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/grwdjmwua.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpqhpzxiv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gdfmtftgw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gzjaxqkny.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gmivnsumn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gobcaafbu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gxzvceauu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gzodjscck.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gnernjcql.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gcwbyoblu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/giwuyakhk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gqpgqewxa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdwbfyoh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gzwfcsmah.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggllgqnkl.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/godhevnnm.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gxykkwaby.sHtML


<!-- 参考信息 -->