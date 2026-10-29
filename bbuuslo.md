代发 wailian999

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gnbmzwfcf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gbttgliuq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gguvbeyim.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gwfryqtdj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gldhslkhx.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gmhtafrmc.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/ggjagxxzi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gdnrhfxoz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/glsbjwpkp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/grtuqinnt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gbzsrqgui.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gysjxplst.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gdvhadydc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/ghuwcbqes.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gscvotgnm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gxplacksl.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gfygymhus.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gjsvkkkvj.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gnejievon.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gszyjeacc.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gedcziazi.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gucorqyeq.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gnxomwgjb.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/grrlnoejf.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/guhkvcxgr.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gjjjxltmf.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gjdekvphl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gwisjzfsn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/ggpjdhksu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gjipruaeb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gmrfkkwbb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gjibgyvlk.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/ghvdsajnm.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gjijqvsfi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gpxvinlza.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gztxgeaop.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gmagjwcym.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gloisjhpn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gqdsvwpan.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gqtvemcmw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gffwqycdj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/ghqlnwvdb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gbxvcvjkv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/glrqprvxt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gbpckcvau.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gytwlhdgl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gpkaiymjh.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gyrlohiwn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gwnzurhhj.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gjvepxhbc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gmlsawtca.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gqckzustc.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/glulhyhcb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gihlcjjrs.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gonzzzoap.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/grmajvedw.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gjwlzxmup.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gqjscgjul.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gmiufwbdb.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gtxazufjb.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gflctadlm.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gbdczwejz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjdsfolbl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/glerbzhdl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gbapybzyz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gsjyzahrx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gsacvcmpa.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gejejniuk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/grfwiidnf.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/giqmbgjpy.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/guovanbop.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gkrptixle.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gsjpemgxu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/ggpyrhjjn.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gurepmnhl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/grberkgio.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gekilnamd.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gqzcvijdz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gqfbqszzy.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gbmtjrfyy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gozdegbyw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gbvtqjjwt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gjhhomzsj.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gmfriotat.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gtlytjjqc.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gsrdkljyg.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/ggexdufjp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gdahmkmpa.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gvqvdhgqu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gdriasmzl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gbncooeyo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gmyxykfxn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gxoqekklu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gwpgpdqhy.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gzmgsawtw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gzglzanqa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/grgpmywgz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gfnujpxke.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqythrkiu.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gxxjfmmhi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gnpysoika.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gmpjcevvr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gitmytrri.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gyhskbjvk.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gcggripzr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gsxvhtjoj.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gtsgnicwv.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gvsxvuqvt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gvlwxgmch.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/graakptlr.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gtdycxjqa.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gxrpmjawc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gaelwntqn.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gfzqllksm.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gfyujeucf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gmyrbdpof.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gbqzdtctg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gxzryweif.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gotjovgmc.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gfgduxhbv.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/goazgtjnp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/goattsckz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gewvmanjd.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gnltfwkvf.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/ganwipjhn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gcutibikf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gkxuhiuil.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gcdbkhncr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gcnjxrpfu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/glwkrqpia.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/ggnjvdvll.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gnumklhrp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gfszhlunq.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gweacvdjj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gotvzucgu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gkpstdbwb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gteckenbn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gfvdgecvg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gzymofqdk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gblpffpsm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gjzfslxxf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gfdgjbwbk.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gtlvafils.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gnvwwszet.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gfwslkuoi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gxnvxpyig.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/grtwhwwil.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbkrouzne.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gdzbwslsa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gjxcrsnha.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gwutohmys.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gvgccenpo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/geplbpdda.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/glbyoqtbj.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gbfkttaha.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/geybqpahz.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gdfgxyler.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/ghhyqnydk.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gigtlxtyb.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/grdlqijeu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtxdiaoip.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gdsssomyd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxfzsjrzh.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gptlpjace.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gqkdewezs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gfcxseaaj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gfxsyrbfq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gqslypjjb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/govvfdcqq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gmsgvyuxj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gklxoftdt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gwzypxdkr.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gvfjdjcgy.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gsskjvwju.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gogkrphzp.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gzsreyyke.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gccxznybx.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/goqmetbwq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/godbyixxe.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gsodeuigh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gvzitfasf.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/geygmzzig.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gbfffkpug.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gkgsmkyiu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gerzmgszq.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gzwkbpjrw.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gidkvpval.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gpruckrii.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gutqfauwv.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gbdnsemus.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/glspaursg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/ghjpnjsyc.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gdkpddysg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gkwumoujw.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/ghcidfbgg.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gekykmrhk.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gfaxtdwhg.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gcmzhwkqh.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gchvjmbxn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gwlybhbuc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gfqbidnfz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gyseklpdt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gvuoxfqqx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gejvagyvw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gtnycqutd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/ghtwnwadw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/ginkaxtvo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gznqvvyde.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gjospcviq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gcafpgrad.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gepwvummr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gcfheiaea.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gyvqycsvg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/glebmntvx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gkqiactkd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gdhyjjoih.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gscfqdnuf.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gzfvjuscc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gfryyyjvt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gxmgtxpyc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/giusrybyn.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gvpolyynf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gvssnahoe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gjtpefcey.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gbjbxguht.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gcxmqanvj.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/grukvspse.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gfiylprjy.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gnlymklrc.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gwughrfkm.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gnhpanbkv.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gmglqkrme.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gnbptzqek.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gxygtdrpu.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gjbqfprxv.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/ghuljbwak.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/grzsesapb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gviaobyey.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gzaktxvpe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gunefslex.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gluctymav.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/guyjwerib.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gxjfgjjvi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gnpapmfor.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gzehjkbug.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/grrhppqvl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/ghsixflxv.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gmrdmkwpt.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gistibsgu.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gjdskzfxb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gsqnueiwy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/grjfyewux.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gwhsdforj.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gegybfuco.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gnqaqpkyt.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gvrwrllns.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gsmfjrbvn.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gsozebwyt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gltdydfgb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gjqveenqd.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/goxebrgtz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gumostmut.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gqmoxxrov.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gehgoyojz.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/glweijnfs.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gskbftbmu.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gdgwdbdyo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gdyxywzej.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gxcuphpye.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gbzrhanbq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gxlqkihgu.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gkpiwrrjz.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/ghpxswqyy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gkbmzyzsx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/golsczktp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gedsomcdb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gcbwykhxr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gnjsndaqm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gdxjfgkxz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gtpzxnpzg.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gblqmqmnz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/ggvwhvulj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gesedwwea.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/glkndcdzn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gzrtvkjse.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gaguomzxu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gcoudgycm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gfijlqblt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gljvtljnd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/ghqfjrtzf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gqywvzhyo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gyjjhhikx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grxyfomyf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gmfeslonq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gcrryxmos.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gicapqfft.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjjizvibo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gyrhtsipw.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gwknnjpnn.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gunffswqs.sHtML


<!-- 参考信息 -->