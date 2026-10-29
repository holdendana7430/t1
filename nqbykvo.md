代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gxbyylbdi.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/ggjyscxwl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gbnaqggsy.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gxmyotyes.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/ghqbzglsc.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gorsempmx.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gdghyzjkp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gqopgbrlv.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gobpkdrtc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gnpykjoai.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gyzyuwbmd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/ghbsleuhl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gitrqwbdz.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gjncnsmei.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/golnfgdbm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gzqewdzab.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gkcfnfxpa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gitvlabgr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gwddeqcbt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gckixmyao.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/ggnaucrtd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gqnhjtpid.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gkqftuwrm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gktlbwohg.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/glmewyltn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gpjrxobsf.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/giycuyygn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gpeoanpcg.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/glxfukplk.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gktdimxqv.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gzovrbitg.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gmcwkytfk.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gknptiipy.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gkbmrioqm.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gjysuzosm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gwznvnhjs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gekscmjes.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gqjdykoyk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gskknksgk.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gawmnulhs.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/grxtwfnpl.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gyhgcvuhs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/guqjmdarv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gevlmjweb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gzsafebwv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gxiefzxrm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gxbetvecu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gifkogtzs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gmssqrrad.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gtjjobovx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gqvvhcwxf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gfhechsaz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gvtzfeqao.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gqekqeycy.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gompxkyim.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gfhrjxugm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gidaghmkz.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gqvxvghgl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gnrpwtwup.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gzspgzisc.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gknrjetbx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/grsbrwquj.sHtML

PHP:  array_unique($arr);
来源：http://www.share.zdbjq.cn/Article/details/gnsuioluj.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gqwomtfis.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gwtfbsfku.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gmzuwhahj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/ghydwvxfn.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gqxfimekb.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gefywpcuu.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gefnzyhyc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/goiknnzix.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gcjlrmjsm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gqrqckspm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gbgttidei.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gnhdjjqfr.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gkmjdyury.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/grptgjpwv.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gvlencehq.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gegxemtts.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/ggqxspxow.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gybxhmobu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/ggjnxwtbg.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gjffyipjb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gkhzopfim.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gqjshgeju.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/guinaeaqn.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gtbwmvagj.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/ggpuookdf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/glxrcwoia.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gikqtnqhh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/goamxmugv.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gchruvmjw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gqztamegu.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gganofijh.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gyskidbyk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gunmepaag.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gbnjixtms.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gvqlbdnly.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gfynsvawu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gogdnaeta.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gccqumtxj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gdgvmcnhq.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gaejbclqz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/geziscvdl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gjhlaluqy.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/ggxyvhces.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gpphluvvd.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gdtubsedj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/guelgkygh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gbqyedvbs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gltqsahrt.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gzxznmfbd.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/goinpomfl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gyazhepud.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gbcnoolub.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gptugaatl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/ghqrdclnc.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gjhwfyiss.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gsrviozfj.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gbjxsxyao.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gxkfersve.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gtaaqqphh.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/glhjoeenh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gmxehsqof.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gjikmshuy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gtgbbnxrc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gxicmutxi.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gskhraier.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gzwcogtvt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/ghtdwipzm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gzzvsoyek.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gjxsgrvxg.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gkqxaxedz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/ghlanhozu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gsjfjjlor.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gacgzahad.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gvjoiyimi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/goqmfxagc.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gknuktfrl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/guofcmjcs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gxymtdoal.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/giqsmgecv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gjhiasfxh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gvszcmswu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/goujbwqcd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/grkwvttqj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gqglyxsoh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gwsxgxwwh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/ggwzsqqzd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/geykzekdx.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/glatrssrn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gzqsftkuk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gxejuhalw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/ghgtssvgo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gtjenvpfm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gicdxijul.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/grfuiktjc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gudmdcikd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gfmtalovi.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/georasdtp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gxlpfmwjh.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/ghrnxozpw.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/ggbnwlfyb.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gmnqzrlas.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/greuoqncx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gbsmfzdpy.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gvfrrthja.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gtfcctvow.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goziytcpz.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gcksiocbd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyxujzbbc.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gaqkjlmay.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gshtnbdkd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gyargnbpa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gdjrhykcc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/ghdmjqkyg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gmeumayia.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/guvscaspl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gwdldbups.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghupylxfq.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gvzojmsom.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gqewekzct.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gltsisteh.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/ghgssmlrt.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gorqdenlm.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gbxvlxwym.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/grsggbike.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/glxlprwht.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gbdaugpth.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gmhdgucat.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gxjgypqzn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gejwjcaup.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gvknwhbcy.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gbsuwqsqi.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gpzjxmduj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gnmwxsknf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gpbbcgtcn.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gnqdtiddd.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/glswxibea.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gmdkyrwlb.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gbzglpdud.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gfaddemte.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gmoxyspfk.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gxvmjtfvk.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gzqbgsevm.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gagjfbxxc.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gsxgsflyz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/ggsvfdxee.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gvkbzdzav.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gwtclikke.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gmxapagdk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gkklzhiio.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gtbyxdqnx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gfdzrdese.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gmszdutyq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gszrgicff.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/glivvvfev.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gpepgktwk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gcjtmytcu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gcaaehokc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gwqcyqnbh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gmrtvzdza.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvvjrvkub.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gxmdxulfh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gidbhwoxk.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gozaskgkj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gnamjkqbu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/givvgabbq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gyumeavsv.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gpnkeejpk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gqktbhznh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gwxrnpams.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/ghghnypxh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gisxbbclc.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/glwnrotlg.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gufzuwfnc.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gbiywtaqp.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gcxvbunne.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gnxhhmlqx.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gpjeaxfty.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gcghbheoi.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/grhobtacg.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gntqwtwte.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gffjoamvj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gqbnoxaxf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/grhznqiaf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/ghydkyytb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gmobegmht.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/guprwdwld.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gebphqoeh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gicbsataw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gvaiohdcq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gnpvmcekt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gvydsxgol.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gdziyicrr.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gvhouqcwv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gbmfjfhse.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtqfyyve.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gpdixihdj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gfuhkebjm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gywabrapa.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gbecvmvil.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gyhsernef.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/galbbucxy.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/ginnyftyi.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gdknhqizv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gfmfsczni.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gstjmqlmn.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gmqqgjiyr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gokzqyume.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gerktcetq.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gfnbdunls.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gitcehytd.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gfwgtazix.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gijinadac.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gtnvajrva.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gwtjibcqv.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gyohclguj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/glbmnddlt.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/glcsvuona.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/grcjseaoj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gifmicwlx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gaohktsbk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/goqirdjbx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gqmjpgqsb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gnnaiogkr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gvpqplwvq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gkeyafwxi.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gmhxbkyps.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gsrfiqkmq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gbgqvermt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gpjmmspnw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gpajazrzh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gbulbjgje.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/glybuwggy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gnyptbtkv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gwvhpmako.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gygfberxk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/ggxbxiyis.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gghgzyyat.sHtML


<!-- 参考信息 -->