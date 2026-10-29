代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/giynzeozv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gimpgjwsv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gqubcvfld.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gxesojrlo.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gqgoludst.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gqavyinpv.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/ghrpiwber.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gdkeawkky.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gbemzfrqw.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/ggqaqsvqw.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gxztvewsv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/glfdtgnnr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gacwjdzzd.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/ghahmlwxu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gphznjgrv.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gwdrradxy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gilvfordm.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gmzcjzumw.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gavlrtdur.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gdrmtafvh.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gvlihpsbg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gycmbrpjd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gonrvqalc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gbsrdgglz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gxihpzitm.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gmqcvqhfk.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gaasaqxyp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gmcxtkypz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/ghkqpxjmp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gttquemuv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gjjyudnxw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gfrpcuhci.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gzqesuykv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gawzevjxn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gkyjkxeet.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gvzyswghu.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gzcypiqsm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gcgfpctos.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gpgvqavaw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gxlynophc.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gwttknapf.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gwqggkccr.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/ggcavnqrv.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gcjotclsz.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gjajnsutf.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gldnzvpru.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/girtwayzs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gpenfuknj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gugimdgpn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gaxrokyvc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gwizfqlml.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gswpcavmh.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gitnawlfw.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/grszqjcpg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gjjssikqb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gtennaxnw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gefvmkfzn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/grxudpdzm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gdfawchjh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gjoyjkpqf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gmqkcntqh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gotkxpihr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gxdgohodd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/grsaruqub.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gtecrfwhv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gksnuaedi.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/grxwzqndj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gtumvumlj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gwsmzcdxd.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gtfxjxojv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gdurhmmim.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gbvllzfam.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gadoqwmvb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gwzbczjbp.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gaezkkbqp.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gejztcijz.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gbqbvpxnm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/ggrwvyiis.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gcxttttsh.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/grsialoyd.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/guqdbcjpn.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gxzmmbgtb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gusviuayq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gjnjjbiov.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gppwaccry.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/grdsahiht.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gwncbxune.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gqvvwdffp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gfuldmkzl.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gflnqnedi.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gdofnxjqq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvetlzskw.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gvsvyoatv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/ghvmymrks.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gkolwzwjs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gnmnmvhww.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/glayfkcqn.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gwyzwzlbr.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/griyxlgoa.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gzqxuukdi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/grpwrhhpv.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gekpbouih.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/grusqgvok.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/ggtgvgrim.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gndmwjrlv.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gnshunyrj.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gbirzvapi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gzxqplosj.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gtrqfuqof.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gdgakctmq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gxdbsvznk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/glsroazsj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gyordqxjm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gtmmoveuc.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gyzvlkspq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gshdjrmxf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gjfwsgvjc.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gpgjzmnho.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gsmjsvzcr.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gjfrndufa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/ggiwtopcl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gnzszxxjr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gdtycmnbg.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gargkbieh.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gsqqhbmsq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/glnwvxhat.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gkyrptatl.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/grcispsmm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/grnpiyzrt.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gbcexfdtj.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvidjghp.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gszjhppxk.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gsftwiqsz.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gresrpifu.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gajkmattt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gguhmrzcq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gfnsqyxbl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gohlttkyd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcxpykhlg.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gfdtubfmu.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gcadicnif.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gtgopzkcr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gwvosbvst.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gvpvjpvew.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gtagxccjg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/giclhfjjh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gzmcvkezw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/ghezjmdua.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gifdfcgfb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gmspssexr.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gwbpazrnu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gqlagsxns.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gnreqcnzr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gqaxrfjvx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gcgblkaiu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gnxsnnncc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gidwwmtrd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gaomtzrok.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gmmnepwrh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gybgfdhov.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gkulzxaxb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gduaahubd.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gdbgefrgv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gykvqolyd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/grpaivpxi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gqgwntelt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gjokabpfh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gkuxadtmh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gkguoxize.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/ghisfghuv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gvvpbkqth.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/goqzwjyus.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gwbilgine.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.zdbjq.cn/Article/details/guxhsdraa.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gprelunam.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gzloqmaxe.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gjxbabisn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gpomchose.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gaebgmqlr.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gunfaqkoi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpqimelhf.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gdnnhmyzf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghzhvmftg.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gmqfqdkfd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gfrflbsar.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gyzsldzie.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gaaatlual.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/ggblptfok.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gebedbimn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gbqrhprsj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gdzfwfjxu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gklfgcqzi.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gpnaveqby.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gjshwjezl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/ggppqedxf.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gievdfbfh.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gvfemrflt.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gjhpfthge.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gpqwjcwve.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/guzapdrva.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gqammaumt.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gydwtpbeh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/glxpcdkld.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/goqpfbocb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gizvomeuu.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/glrtijydm.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gbttzmwyd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gscgbvhru.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/ggdmsilbu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmrwytlr.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gmbydxjrp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/grfeojuea.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/ghbzxpfay.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gpzgslxvu.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gctkuyzok.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gleehyhqc.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gulbdmdmd.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gptmnnkfu.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gwyfuyyna.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gezyypqux.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gsvihhjfs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/guwfswhin.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gqalkciwt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gsqkexxcw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/ggqblgarb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gqcjhmvcq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gekvphmtn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/ggkhhhlds.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gvdujdhch.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gzjfydcoh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gwwpkoqcp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gwbuwmhhu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gmdaxlukr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gocpywtdv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqijzmhzc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gvoupgnbk.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gqbzxvzdv.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gzewluvfq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/garrohrei.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/grmpoixwh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/ghlovbcbn.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/ghivspxvn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gewygzvmi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gwcvkcojo.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/guyotcqtj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gznqvdnxc.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gzgsjdmwq.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gzzinnkts.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gxfbwqldt.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gorcuercq.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gcsjnghlg.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gapyqfbou.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gztsfawxj.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gcwbtjtmt.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gdjetajgy.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gjsaoyijz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gjbkplggl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gkvhorgzi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gvdqnujpl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/ghgdqyihi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gjubkenvm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gckxojjjq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gyctjbezf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/glzjipcia.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gtcszydou.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gpromlufl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gkejrdxtx.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gezqqxdcl.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gxekptvcq.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gemnypaia.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/ggibiiskn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gksaweneb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gxsbeofzo.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gkgkvmfld.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gcmmcevjl.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gxfnqoutb.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gbbdtwgil.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gcfekajpk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gpvydyazm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gdodwqwun.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gyyumfauv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gzzzczkec.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gsmzrxqdb.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/govvupwpy.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/ghxeqmypu.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gpwpezatj.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gencvzknf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gncxhopnl.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/grmnxrzxt.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/giezpcfcd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gmmvaawgr.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gqcwoamxy.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gdyphymqw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/glnzrxllz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/grrksbrbj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gcyfnqvrl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/geseoznub.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gtoanfcxu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gapdhauiq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/grradaxej.sHtML


<!-- 参考信息 -->