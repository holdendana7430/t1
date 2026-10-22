代发 wailian999

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qxrhxydr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2kblsdvci.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kvipfvqp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bpjptlaz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2zpmlsqhh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ptmqhzva.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wkshcfly.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2tyvghwdb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ygdmjhie.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2dgyjyhtk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2suboecgt.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ecqicgan.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2smjyfjdy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jqaeldbo.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2nkyzmbar.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2tjjrtmmw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kruskfsp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2lachfpuw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2hdmcawoi.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2kuljmltj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2szrbcldd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2mhjqzbep.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2tdmjzvgg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2vmnyoaef.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aeribced.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jpwxkpmf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zvzvaoaz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ehszbxax.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2olemdqjc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ykhuncui.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ssxhepgz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2iwztuood.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hduqedye.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vdyeugqk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2vkhsjlrx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qhidujtq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qbyfbktq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gytvkkmg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2uqelnauc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2csarquyu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2gwmmduvp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2emcnktix.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ogmodxbp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2gjhvhxlf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2njyjmqdw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2blbgrvgk.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ssqxwhfq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2pkylisob.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2btflsrlh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2spxlcllc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2pyezvmlp.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2bgmjhrgv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2wbhxtedg.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2nmuhsstd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jobfaeor.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ynxuvzqb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dldxakvc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sddlunvd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2dtfzaiou.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nhqkirli.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2slxqdmvo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2mwoxxncq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2fhmfnqxq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tlciwsfr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2mhfpajxq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jjquzczi.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sjdyicrr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ssmqfxol.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2kampwurt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2gtjkvvlf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2obccbllh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wisrufqk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2gbnuvdih.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mcjnbzyo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vfdexxjk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lxyfzgzc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2isaugqzw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kbtptzed.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hjfyxsuo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qyqwwnic.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2vytzztia.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2azyogtat.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zhnfelrt.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vvopqtrn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2iamljxpe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2olivmnwc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ekyrorwk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2mpuzwanm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2xxiqpmqa.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2bwdhjnfs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mrkosvpv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nkvmtucp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2odemkbkx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2itnoskrp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2hvmmtmct.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2tqziuonz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2sqrbdduu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2yaexyyal.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2fkmhqiyx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2lvzccslr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gopahcdq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2hbvuazup.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2spqzoair.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tzdixquw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qbtplmqv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2rhigvqny.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2nhusmknw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2zphattfd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2hmckbuso.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2lxherphe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ljidyrez.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2bqdlqbpt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ugsauzro.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2adjpscwo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2pglunkye.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zbsfjtmg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2vwpeexim.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dzlpivjh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vjisfith.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ljaefojd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2oztxejbp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ofbjsart.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2pqkisejm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2secilxsg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2euiblsxs.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rmmgibcp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2hnufatau.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xpvstyve.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gieddklh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gjzkhssb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2yyregpwn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2eamsqdql.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2idmehsnq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2grzllgaq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2pcskovvh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2mtsfrink.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mwuqaeeh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tljsglai.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gdtmieim.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jzcejxee.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zhzuxdsx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rfdzxnuq.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uvcaflyy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2xneodhhg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oplpbjiv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2mytrsxhq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xomjkqww.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2rsqpatse.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bhlbzggi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jtwxygsv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2hvnivqog.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2oqwnjfqt.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2aujlhbof.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ikvbwgqk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2krmxdvlm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uvipzvsl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wjmzrbjv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2lforrkfo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kilxivnc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2kdyjlhgx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2rwnnvtfm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2fwowavol.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2abgbzpwy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qbkemamy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uxhjaxxr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bxccenoj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yzluytbe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2eynsmlym.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2bliyrxot.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2tvdyujvd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2nelclmrm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2azyrqqkg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2yztjqdnk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vkypxhoz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2uvorkyhl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zoqmndjw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2obpzghjs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2gexydgou.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zpxutfrj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2mqfftzvm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2cckmataf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tbrvoozy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ovdodque.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mpibdkgy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xnosocsy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2qtfdsech.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rjdbgoth.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2awxmlpwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywdxkred.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2rgafaumf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aoegaozq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ppnqekfo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2dcojjdst.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2lrrcwxru.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dlxyhtis.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2onhwnpab.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hnykfbzj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uxbsbvbw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2zqldihlj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iccfqppw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tqbqgohd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kitvjmok.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rghwmlmf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vrpourcg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2levyebjl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oivcsifg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2pnfyqfgd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2yyenddlq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2aaphvezq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2uaykbtbb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2scodiyxo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dbbxjitd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dzffahjj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lecxkceh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gtkqmdll.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2scnzuvcx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2opdchuwb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2aqttoqbo.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2czzttupr.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fyazlege.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2qrewmftm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xgojhjtv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ofzjqhvj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rlobsccj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2zmtivect.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uyktpeoh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dwullrpl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2qlpphkot.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ygpxkotw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jozzslmi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tgvslvzd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ewmoxjsd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xaadhuah.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2uojbmbif.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jhpjynzi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2smvsfhzx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2azcsgswe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yztitjga.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zxdpnixl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gdgolpgb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qgrcjwrw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rtaxxkuk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nzblhccz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2krjlnkla.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2miuhafdn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2grjypsvq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2oxslkhaj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eltdntgy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2lpztbjgl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2punojyzg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2mapdjyxk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2cpecbqwb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2suelocbz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2agmremvn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2fkryhmqw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2fubutngw.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2msadzfba.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2llsgyept.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kaogwzau.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hipuyugp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ssleqtvk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mefdvjjo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qvqcnhzl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2icyruyzs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2kbmndfkk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2czepxyht.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ylmerceq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xtpgjpeq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zxwbokpt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2vbqjuokd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ohmvzivu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lwdritva.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2cftxhtgk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iazbpkql.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ungwictr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cjxaectb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ubisigti.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2eyublyem.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2trxstvet.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xfwrxzod.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2yaqvpbup.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fjmtoxcj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vugpzzza.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kvvbrayt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uihsagdt.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eveacsgj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2wkrrvvuh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xbbshihy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2nyetdemz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2espqprjp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2oqqnkbrd.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2pyyekxcx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2uddiqsbf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lvrynmdu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vqssztel.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ruhojcqn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2btzldwso.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jgejared.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2jduosuym.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hwhfmmxw.html


<!-- 参考信息 -->