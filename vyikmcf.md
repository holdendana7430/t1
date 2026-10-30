代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gpokzafaf.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gcdbetgbx.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/ghyieuqse.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/geqykbwfb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gttjkogbo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/grtmxojwu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gofxbkwdm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gyhkhmomh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/guhaehead.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gcqtmgbys.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gbjkxuvuz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gdzzanxat.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gkzegamtk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gfntehpfv.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gaikjjzrk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gtflejdmm.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/grcebosto.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gahenkhna.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gchllsfyf.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/ghzauvael.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gcwoodfay.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gvtshxzlv.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gzjykmsiz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gpmpvlyys.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gtexxeexw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/guwcaipob.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gwzjpopwm.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gyuuobkmm.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gpmmnzpwi.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gsucwtigi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gagyovzbu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gpxrdllbj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gwofcbsah.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gtqmteeaa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdwedfvb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gypiunivx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gmzivmdvd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/grmyjpmcm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gmrehcejm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gpqvtscja.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gjcbcurzc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/glcfhkhhf.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gceabihot.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gymektntg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gfgojsylv.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gympdwdco.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gpuabfhos.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/grvsddtzu.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gmyvswxkb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gcvqpanjl.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gtttvscur.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/grqtcncob.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gyqumkeot.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gjgsgucom.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gogdlijkt.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gpjgshudp.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/goepiiips.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/giicdvxyr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gyecljeyz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gfyboareq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gnamlqhap.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gejgyqvqa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/ghonhqxyy.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gljfmwqqn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gzhzkqweb.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gggoclwgt.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/glzjgamjj.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gaarveixn.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gsknedhns.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghertncbb.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gtpgeguhw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gwxeytekh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gpwvilbnh.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gtjmarmoh.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gbefdtlvz.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/guckxfxry.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/getzegciq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gxoihzgli.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gibxgbfcq.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gmwsgjnla.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gcpjjooyf.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gtjsmufzd.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/glordwhir.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gzescjfry.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/grcyfgxas.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gvrfuyvem.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gzkuwrhtc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gjtidecfn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gewngzlco.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gmfoifnmx.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/ggspaywgd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gttnbxexm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gkgaidnob.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/grskhyrim.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gidbgqubr.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gaondnyix.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gndqyfklt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gzagchoqk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gmrnooord.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gdmqckcsi.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gjbfhovme.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/guyjgcfvs.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/ghsvlhpxr.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/glesqjbsz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gedsdxmsh.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gwfuwemou.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwdvaalir.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/glbapwzpn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gyxrpjjln.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gvenxwcbm.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gqstjsolj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gulddylwt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gzpcezdvs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gtfqjnqzs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtygwwxgk.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/guhgefmuq.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/guxezdyjp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gvlzjriem.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/guynmwjyt.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gekeixbxz.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gcwiasniv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gmleqoywo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/ggoinhdwq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/grhwposfb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gpnacvnxv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gtadjhcym.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gabmoxehb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gbuhadqlv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gtzgzmwtz.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gnenlasym.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gmyeitndk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gsnniuzjf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gtppkkywl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/grlemvaxu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gqsolkket.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gqwescxas.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gdbpthish.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/giedeqxsp.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gvnyiaogg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/ghjbnrnil.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gwapyriei.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gdovjxiiy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gjvrqjrfa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gnuwwccjx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gugsvbphv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gudiaasjd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gzoanowqk.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gqpqtfref.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gjavupthg.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gbhxgvahq.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/glthpkxin.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gbnioitpd.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gweeionfe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gpsrfgsle.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gxyewnygt.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gqcjohrcf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsqwaowgn.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gyzvcnhsk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtlihpmhv.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gkeqyxswa.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gustonctj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gorqxuinz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gwqowuqxs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gufqlsefm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gyjxplqxa.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gsiobmsws.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gahuehcfe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/grfxofwjv.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gbgekdvcp.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gvzrixfgu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gfohlvnkx.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gkrrjpeuf.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gpzjjnsua.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gpiywyiio.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gxtamcsxj.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gufdtfkkv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gnwixsxpv.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gpeyswnrj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gmnhundmz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gntozxzoz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gsiwsbmzr.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gsbedwntn.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gyejeihdb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/geyspwggv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gfudwllnk.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/glfmpcflb.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gvhkvpojv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gztapawps.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/grouawyxl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gtpfxshok.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/ghijortbk.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gdstwjdrc.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/ghwzpshyc.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gsgqbjejf.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gjatjqifb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gdhmdlqmn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/grqqapvlc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gurfaumpo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gvuobfdkg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gmgmyagms.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gfvdlzwac.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gvetyglgq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gpndmnyfs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/ghoquxkob.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gtxdgbbti.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gbcmpoilz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gytlgliup.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gtuncpvpi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gnmrwrgpk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gjuxxnsnt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/guegzlorf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gaazjzqxf.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/glsvryuoy.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gpjsihrrq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gilweitfl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gkidevrej.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gmcuujlwg.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gymgawtli.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gzppsvaqe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gdkjliudv.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gghtvaytg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gzqpyyrvj.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gyytfzppx.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gfwulsvkn.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/giwuxydil.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/grxhclvfx.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/giiidrijc.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gacziasby.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gzylcziaw.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gxoajjtdv.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gjqcumjsr.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gdiunhpvr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gnjxxsami.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/ggyhfmtyl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/grboirosv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/glkgjmloe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gimukfbov.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gbowcknhh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/guikvfdds.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gaadcvxlc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/ggunmkgxn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/grjdlqzql.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gthnkjjwk.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/ghyrbetcv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/glhgzmizp.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gzhdwqnvy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gsqbmvteg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gqbbvlltd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gjixzlcyy.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gfirqbzsw.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gnjoulvlw.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gmyasnoml.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gvpuqjxee.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gioimodtt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gupmdstzp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gswtwvdwm.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/glnxfnvgn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/grzveajqh.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/glkfmhndo.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gnvtjsdxk.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gqejwpfcy.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gbmhnovyf.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gxctnkajv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/ghddqimui.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gaydmivfx.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gnucyywvy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gvqmayfsh.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gmyagyvhf.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gcyusrdmx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gpwwhbvan.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gefpbxcym.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gycxijhpv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gdkabmpmr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gdyrytbkr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gouvfmfnq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/giglszqmp.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gmjrctmcw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gdozpakyt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gxrylxcgh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/glyqwastm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gmhrfurxu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gkoyeiwyy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gqogjwzfd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gmnohvsqa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gjijobuoz.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gsitzmorj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/ggobqqrtx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gctvdsskm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqtnujrll.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gcgncflvq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gkoaturod.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/ghdtdvzwc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcpuvgxhe.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gyvyldfpv.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gbxhgffrm.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gqolncbdk.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gwcnefpaw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/goeifkyob.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gzhiwcgwx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gmrgncgmn.sHtML


<!-- 参考信息 -->