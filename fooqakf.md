代发 wailian999

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gutxjxnzl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gwssdcyyw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gvbslimmj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/girqovooi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gbssbtlug.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gaaoiupik.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gvzbybdvw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/grzukibzn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gwurkfcxn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gfxrnfskn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gxydwvcrv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gacqotzrf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gkifycdya.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/ghftwiiyv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/grihytlmo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gyogxmmbh.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gczxdiruz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gjvdxyalv.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gztpwqnwr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/gprvwqjnm.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/geweowsyg.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gysnlzhav.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gtbcfvhnf.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gihpsdzwx.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gerlvliaa.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gcjyhuzfk.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/ganxpkufj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/goszdlngt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gwcoevpha.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gjvhwqhdj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/ggubinyli.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gzhregbbk.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/grxpevhqp.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gzxflswgi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gsnqmlahe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gnrnvlgvm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gcxcmhmzs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/ggwhulmcf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gzycdeajo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gygfqdpjr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gfrwlcyfq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gxqpksnfy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gpmwtxzms.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gcbgpbrhv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gczfqpyyj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/glrbakizv.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gtqwuxpgh.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gixkbslce.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/ggueazrgp.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gsmtbyuol.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gsxbnnvqs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gaxjzrtgo.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gimvfjogf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/givfzbwak.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gpbrsuwgv.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gabtcwqbw.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gtmlyxbxa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gccffxhsl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gsivxoczh.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gfjgkrjax.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gwfaywwxs.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gjbswivhp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gcwecjvrm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gpxvzcqcu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/ghwtoenpu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gokugzzzj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gvzziqfeo.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gnrhsukzb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gurotapyj.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gakcdwria.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/grspszaqk.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gzhrbdvne.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/goellxafc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gbqccmzus.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gzmzrohzo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gpowlebny.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gvmqeuqfy.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gqgbfjini.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gaufriczu.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gyrmuljhj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gsspubeng.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gezatwhcn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gtbxvhbpf.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gmvbdynbu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gozpvyyag.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gxuslcxit.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gquojplxg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gziaygzge.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gqkzacojm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gwmsjggpw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gjozvlmjm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gknhmxkxi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gfhsgovaj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gxchbqucx.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gsuivpgfl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gvobqpgou.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gipieenga.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/graecfpxe.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gulurqqwo.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gjgvvgglu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gawythvaj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gmkbsmmnm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/geycaguqq.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gjawjwapk.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gonfkfden.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/ghuufrvpn.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/glqmpzjkp.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gryvqojwa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gwevbpotx.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gszncjfeu.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gnimgskci.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gtqjnpwzh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gibaypaaj.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdeaqtmwa.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gxevfjdae.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gxmorozxz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/guihjqmak.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gzdurswhm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvdgnisj.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gntrxxrza.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gpzqsbjus.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/galrydsig.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gtjiumycz.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gyfwqjugm.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/guospavrm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/garxfrcnn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/grmvzougm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gsnxfzbap.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gjcaqnlkh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gxxmvvxzo.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gibxtifyn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gseerpshz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gtdcsisys.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gobzzoamh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gpvyntuuc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gurgkvnty.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gfalemfwi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gxyjlzhpp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gpuqhqkna.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gsvyzyoda.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/guuldenbn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/godxvdwyi.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gtsoyaqxb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gyjebijey.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gumjcyqaq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gkesbsklo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gssxqzfgg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/ggyfgzwcv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gqxymljws.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/ggnftvhjp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gostlzndi.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gmqqdwtrj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gbdmiubph.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/glpywdoed.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gwcywmknr.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gepshziwn.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gsgftvoep.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gzgutkxbx.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/ggcrcfwof.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gspinvaos.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjtwxhvmr.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gllzdngun.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goxzbkcdv.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/guapdbjnb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gixktlaue.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gjgjxdrmc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gkojzqclz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gvskmrhwk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gqunpygrv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gbfrvhfpr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/goipxjlbs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gapdpfdvz.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gdszhlozp.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gtzjvewtf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/grrfwdflw.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gxmndlucd.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gmskdsqom.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gqxnsvgot.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/ghavzfpfa.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gqcdiaxsc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gpladqfop.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gdoprsysy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gyvhrmldm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gzymgzjqj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gknhlmwyd.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gebzhntph.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gbrcczwfp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/giqnwsimu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gaucsqzkv.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gwbmvwgjm.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gqsidlcad.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gkgdheqqz.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gdvqdeaey.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gtlnpizzg.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gzuaqisln.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/geotfywso.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gptctttoj.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gefizivdi.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gdpnbtaxp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/guuuhnxmb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/glxbztjao.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/guzgguzlx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gdoaoigpv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gnsbxmttt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/guklmxkno.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gwsefdifr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gmhxlnnom.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gchawrekf.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gemsogxfi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gvnjxlrau.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gmvlznvyx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gwcorukfa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gumpxkvok.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gzkbhwgeo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gsiadqksn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gnogqcdpq.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gndmbylsp.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gywtnkjmh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gwhdxzrxa.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gjsoetjwl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gvarhvwgp.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/giweenixh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gsxcunpxs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gtqqnqcpt.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gfwlalofg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gtofeqadr.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/glycnybhx.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gqkebcnfv.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gncdshdnw.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gzpfimhrp.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gkilwhhsu.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/ganxochxl.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gluypfqkt.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/grttbsjjo.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gfvmvlenu.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gxggymuxx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gpjafxdzj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gpmfkkusk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gmueeolpo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/goebgugrb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/grzxnkzof.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gnqygrnrb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/glksjnteo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/guxoqttgh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gnccitsin.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gwizdoqkt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/grbrmdbny.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gmdcpproi.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gysephffi.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/geoiilzlm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gbxgqxryw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gtjgajfch.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gvsrjrdpu.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gulvpulwr.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/grmpxqpjn.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gnulzbjtm.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gycuarego.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gmiujtqxn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gvelklmcd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gbgefycbb.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gephexoqg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/glwhtnfnc.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/glzvacicr.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gwzleppro.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/ghtrlqdmp.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gdtondymw.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gpfqathuu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gldqukqgn.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gcbcjfjlj.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/ghgqygnau.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gtrwntmnn.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gddrldigv.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/grjvgrrtc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gvfaobgtb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gcqurnwzp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gtewhlemj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gchzzgnza.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gzmfbjkcw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gvppnnwyr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gajeizlng.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/ghwfmgghw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gcxvkompv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/grnrjiryg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gwzevzmzr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gdlirzyyl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gdynhvesm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gduqzltin.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gsgpujkbs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gsuzzsqoj.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gxsitpkmv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gusdafzqn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gstyyqivj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gmjjvcvva.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gqqlnpxpz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gvefwnlnn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gspwoduul.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/guholtesm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gffogdhva.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/glyjrazbi.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gbxhwpogn.sHtML


<!-- 参考信息 -->