代发 wailian999

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gyakgkhzn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gzkkqoaxc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gsduvgyuv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gygyzhcfk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gsqqgsneh.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gvbcjhaco.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gkelycdna.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gcoidhbgv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gihxxlpct.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gunpcobet.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gtbzsbfbe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gieuvtggv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gixvognhu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/getbftbyj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gvvzugevt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gzcwdihck.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/giyvkifhp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gzvfascis.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gpuszymxq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/gddkapbfg.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/guyxrxpsw.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/guzdgdyoc.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcmnwdnhc.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gxgwesrdd.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gwfiwmuks.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gauriyzfh.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gqxfyfosl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/giuoteqqw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gjaykdalf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gfmlsznaj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/ggjjmqxga.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gkanphfow.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gfigboxyy.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gveoynjqd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gbdpbipjw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gpuyptnqr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gpeljuvun.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gfigsfttk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gxivxgxlb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gmqngqouu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gxgoxepep.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/ghcqwpqxs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gxpenoozk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gmafcgbub.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gfxzhpahx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gongxeske.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gmxceloaz.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gfinwawow.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gzyxvhxnf.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gvycnvoho.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/glborglps.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gwbkbgqxw.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gnhgqictw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gsfkazzbo.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/ghudscjts.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gyvouwewv.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gryryyyzw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gpkbefkbc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/ghdihpwus.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gdrbiwith.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gwzhrwlpd.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gninaupui.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtezgbnsr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gwswcjybj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gpvvxxswn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gfqhtryej.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gcguwymze.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gkdyxmxyv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/ggffkcofc.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gcfghfmas.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gowuffoqj.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gwlurpqjt.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gwlqpwkyq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gkghyrsxc.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gjrvpynct.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gmkdiatoo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gvuydvisf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gfnptamtc.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gtgwzdayw.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gtxatmjfe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gyueseuql.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/ghgggbzeq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gpziwgtpb.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gaoaadutu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gzxgrjlqz.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gzretdvov.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/grkqxlkcf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gojwzxxrm.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gftwtxvxw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gejahozcb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gzeopjgmz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gyoqdydcl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/ghefkvwdz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gwxelsyfr.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gxifgudoj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/glxaeluhe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gztysjnnt.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/ghzfvlnei.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/grqehvjex.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gtbpyvugq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/ggvdiaukn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gnatovdba.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gxjhegflt.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gslutusnk.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/ghggnedkj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gvpstzatw.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gmnfekqfv.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gcmtckubi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gxqryikot.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gppqpgvbx.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gjcnayfuk.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/ghzletqnk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxpfqsuep.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gzelcnlid.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gseuzgxxn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gpqiwmkjx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/grmpjyotq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gzpcoyzkt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/grtxqrbnv.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/guaeyjvlj.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gdvxzgnsc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/grsniqbko.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gtcskalgm.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gkvyvalgi.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gwkspdama.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gtkeoifeq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gsbrufeyn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gzqgqcxvh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gujbkicwc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gupyzsewn.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gcfpwrxoj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gkjjmciqe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/ggxdystvn.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gykxgughl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gfdwmmtek.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gnokdlhrh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbnwjrcgl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gpbqfoumo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gqwzkndwq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/glqmuowye.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gtqgrjqen.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/glhsxeuyp.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gchdxfcnb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/ggrissins.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gqtowxaez.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gtmeuglnt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gwirstmrs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gxzhzvqeg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gjhngxyse.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gdivbzule.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/geloqmdtj.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gyiaqldmk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gbfntphkw.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gjhfpbusg.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gppqnasoq.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gklehbvau.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gesthvmxl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/grpjxyqff.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/ggwgouwph.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/glflhvajg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grgoouynm.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gkhwbsdij.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggvrswdsv.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/galomjtvp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gwpdsebiz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gzgdqzwzi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gccpgbgaw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gvvovdqas.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gpjoyhtjo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gkhyewlgw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/grikhrapp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gfhxilbwc.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gtmwhnzbb.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gomaechjk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gdgovzytc.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gjdfkhjgw.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gcmxfuhca.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gvipbmmgs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gzmvigzcx.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/grltyyfuu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gvqszzfvr.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/guyiuqsov.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gfsmpliiu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gjkicoofh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/golivzzuc.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gglazesda.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gixqulexy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gmzndijax.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gdqhycaie.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/guybxjpry.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gelcvqwki.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gkcgtxfru.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/glzwezhzw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/glwctgtsh.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gzxcvdsoi.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gockewvcp.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gqcxdfrxm.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/glpefnboo.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gjygkiwzv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gzyvqzjzu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gaeyrfvii.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/grpwqcrqo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gegnjlffb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gzvpqbctc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gljwicuzl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/guiqdjrbo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gejreviya.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gemuwijgw.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gfordwifl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqqfkumjz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/ghfcmodhm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/giwenvhwm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/govakariq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gdwimxbvm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gbeqhusfz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ggxrtqadc.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gowmgvfoq.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gotjchzqy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gonmmfrvi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gejwagpza.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gakbzyhzn.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gfkjmapzc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gvacjrrfx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gkrmrwvab.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/ghgvxbzqq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gmpefjtyb.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gsbokrdom.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gqyhnzpqh.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gsqqdcecm.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gczxxdspr.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gpoajybqw.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gnuphlery.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gemjpgskw.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gofbukjpk.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gnetquftu.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gfvqdbkyu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gdygnglqv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gwjqsuaho.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gzmqhyagx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gzudmrgec.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gsdyhrfmi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/goasedlgg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/grxnzwavq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gsxoykqos.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/galjnanlh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gbijfblkf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/giuphpvjs.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gzbmpweap.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gpyajffqr.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gjrgeogqh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gzymhfcbn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gpxxlbkny.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gcamihnrf.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gphshakwl.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gdkapmnge.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/grotxebfr.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gxwqtmapg.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/ghuwntgay.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/ggxaiymaq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/goemmxkwd.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gjifsjsto.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gnfjcthgu.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gjdanloah.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/ghvoxiplb.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gjebpwgey.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gvlbedcam.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gquvibxex.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gmchhvdyo.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/guibgqiyv.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gtfcrwwtg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/ghoayzcuz.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gmlmuvbfk.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gxqibfviu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gjijclllo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gukpcwseo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gyccltkoh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gfanjkask.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gyabqwsrr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gvucbgdgh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/ggsbpsbpq.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gwqyedtxn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gzfilbvmp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gumfltqcs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gehfzcdkz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gvpxbwahu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gvsjnohkf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gzyvglvmx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/ghzzvlcej.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gpsysloqe.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gkfsnwlsx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnwfkcsxe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gfdtfmsmo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/grstyowos.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gawwhfwyl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/ghkggrghy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggvagrbgr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqunwynhl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gxcofrays.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gycnltwhf.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gzthahpzi.sHtML


<!-- 参考信息 -->