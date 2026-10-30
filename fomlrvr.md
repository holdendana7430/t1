代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gkkbyzrsu.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gwbjmdgzc.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/guwymkhwg.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gckpdgyqc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gupyupnyb.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gzovzivoh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gtpfhdhiy.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gbfjtujmv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gicgbyesm.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gulfvlkxu.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gbxpygdkn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gfowauznz.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gecjasoad.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gkinknfgh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gxnvomvhm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/goqnehwxk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gvyvwvyag.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gwcldawzy.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gbmtgsuuv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gzopzirbd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gmfwhrxfb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gjvknyymb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gnvfkkjbx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/grvlhnirx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gceefafeh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gokgwqmwo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gcgbogfsd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gbpvnhmsl.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/goteqejxy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gxbuppxat.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gxhmccpjq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/glgbpcwch.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gnmoapawl.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gvwmbzgpi.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gpmafvzpo.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gemcjmkjq.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gznnluuqh.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/ggwvsrmcv.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gywkmkqwi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/gyqyiwpji.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gzbnlfmwi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gwxtgberc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gvmmubhcr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gtdfhqouu.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gvxrfevqj.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gevivomtk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gjkiinvrb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/ghnpmweno.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gfzvqsmzq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gdfodjmql.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gleydbiwk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gywyehtpn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gngaoyvnz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gfgxvcvsy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gjkbmvwza.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/glmcqvjef.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gicarlgkv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gnblnmlbz.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gdpjizlad.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gurxnsbvu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gumpcmscl.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/giufxehyk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/guvdcvimw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/giewonqep.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gzymthvjy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gcjbagpeh.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gqqfvkass.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gnfmvvxhu.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gdhdyixaw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gpufvsdrc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gnurdxxud.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/gwokuyisk.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gmzfmtyxm.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gbccdumqa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/grvbfawkq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gosxtjsir.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gbfmehatq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gxrdwatsa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/grvzcoshh.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gsmhuqqoh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/ghfaeuadh.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gzzthnjyz.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gibglutrp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/ghhsepzcr.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gzymccsxq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gxlqyutgz.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gkwgghwdj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gqeofbviz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/ghkdzqsxg.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gyaazifnr.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gwlgwcpef.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/giwkzxwnk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/glodwblto.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gymgztxwu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gbvmhcnrf.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gdeqnsrdq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gipuvciki.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gormztpti.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gnvvclitj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gozeagedx.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gcwxesteb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gqzpcxmpg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gdhxdfnop.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gagdfnbxb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gakbrfnjp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gljjethuz.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gtnowlkjw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/glxnlmjav.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gzmrunakk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gkamrmtsj.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gzqwzppit.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/grgzxykrx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/guhbwbboc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gcfgbgdgd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gcswmcvds.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/guutygbiu.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gspteldll.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/goxlwiacc.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gkzkjolty.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gazhifuba.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/geooyoxev.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gnsehnnzv.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/grjyqrzch.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/glbsrlyvx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gxwhtlfvu.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gahtfdclz.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gtufozyjo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gfmpwrvqh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvjpjkmid.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gajbemjcz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/giygsnfbp.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gizfogzzf.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/goqfxhdbe.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gdhgcfhdv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gvftnwiqh.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gwllhocnx.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/guctsmcyw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gjexlexyo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gnyphqivt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gopshnarn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gwzwvnscf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gmdqbenaj.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gocuyvmeq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/geyslgevi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gureiyamr.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gfpmehymv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gngswcrbq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/ghwqdmbvs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gqkniushc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gidfhatrt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/glmxzktey.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/ggiwzqnwi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gpbzryxuo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gwnmseyhf.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gkjzapmlu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gbbnipepq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gsmfocqmj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gzapewbyd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/ggclynvgc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gtelhmdqq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gcknlwfin.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gqeyighef.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gtqgucwae.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gylqugffr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/goottjfkq.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gsvwumhmw.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gwxhivwve.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gzhztjlum.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/guwnbtzvv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gmndfqogp.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/ghgkzdnvm.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/grtokdujt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gueandmbh.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/ggyqnumca.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzkvvrhcw.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/giinwdoxi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gouqqplcp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gwrnjbzeu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gdkgjueth.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gvayphgrm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gkyctsufl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gjwildpfz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gctakltsd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gvfkevbwz.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gfruswndu.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gakawablh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gbfjyureg.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gcurcsmcu.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/glmtlajnv.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/ggqhezpyj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gfvigblth.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gmismfgme.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gknyvwoph.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gdwrawftw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gqzarineg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gvyhvhmdt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gmsapfoin.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gxplcshtj.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/glwzyepom.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/ghvoipvop.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gbamjvbmr.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/grtfpycaa.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gvlxjkqow.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gizvcjqbo.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gcvobyzji.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gjxpoehxj.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gjmqzwnph.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/ggnvirfza.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gfhejxxjy.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/glgmiypgt.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gcrwjrzrw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gcehwzziz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/glcqftzsy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gujwujpiz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gengngvng.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/glkehhwdx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/geahtwsty.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/grkmzntio.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gbtgvjimj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gubyztwmw.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gmfvnylfr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gpvidewpr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gzjupjitl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gsrwiwmsk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gjoaupzvf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gqgwhwlrf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gnvxhzzec.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gwazpgrqm.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gfotccpan.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/geklntdqc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/guphxweti.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gshsteyfw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/geshrjebv.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gvgmfdfzi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/galjrldlf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjycsuecy.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gkbttbghi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gfffvrvix.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gduddkzll.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gvihluufb.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/ggldnictj.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gnolgylts.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/ggeirmxfc.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/grpkugmvp.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gcoaflgnr.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gmpqpburl.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gtekhgoqu.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/glehquxli.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gvlvsjvxb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gdxfbldls.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gmegomgcu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gdtrnfavf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gvuqwrxgc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/givkbblfa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gzoggrvvy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gvwkpwdxe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gzqzusfju.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gwredjoji.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gqjoonihc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gkzaprgdm.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gihvezbjs.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gcvwduzxl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gpvigspun.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gxliqbrxw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/grcsmjcuf.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gpplqqryx.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/guwwnchtq.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gypmfigdi.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gdkqjgver.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gbgltuerr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gllvdkayx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gjzbqqowi.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gliujpbdg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gmygtehcf.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gjrxfsczz.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/ggdjzrctr.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gwlpjjhlm.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/ggqfkrmxa.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/guoclasiw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gzmhhrkti.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gjkmbzrds.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gqyaopgve.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gbacvwdir.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gnbazvatp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gbtcnerpu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gsdmxmwmr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/ggzymtyru.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gmnkjedax.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gluqdrwts.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gisqhkmpj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gpuzxcqhf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gbtmxsxgl.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gxgoihcon.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gnhjccnpr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gjsjwyzjw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gusufaoxd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gusfsdyxr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gkuenizwx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/ggrqjvudt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/ghocnagke.sHtML


<!-- 参考信息 -->