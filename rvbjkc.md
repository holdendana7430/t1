代发 wailian999

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ueexuyat.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2huvwntns.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2cajngmsg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2nvsnstmp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2pojwegnv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ftamorfz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ehsiyhru.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hlcvlnlp.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hlfuiyqq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bsbhmuty.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2buqbxikx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2nzvszvsr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lihdyxgz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ymkuzavd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2zashhdrf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2zrdbxszo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2lvopwbpj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2sgwunqkr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yccohbpy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2etdsacjy.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2azjpucoi.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mfmvcxky.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2hlceuvqw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qeklivak.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2iyyavhvi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2xbpvczgh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2jfcqufwj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ldsmybon.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rbbdbvuz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rdjingig.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2pclvmmiw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rrrpzojb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lisfyllv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2efdikogo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uivredxm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sjzljfdm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2pulqiwwu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2qydnegtm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kbhexgoh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2xiwjdxss.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2olkdncob.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2iexwttrt.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2jtkdjdpu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2qleaqmna.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2yqkrkwoq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vvztmkaa.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahqnghom.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kxjtoxbm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2svgoedce.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2boppgtwv.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2udirxzfx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nwewvevh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jwaghkem.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2plxvrlny.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2azbgklur.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mdxjyowz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2wnqqxvmd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ozwqzzfj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2kwbknubs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2pzrgfpho.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vmcirzei.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2likxovqr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vijhoczc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fftdbgqh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2joqbzysh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2uavtahfs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yzwlkjbv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2afblovmt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ezpwagat.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vkizyvwj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2tgqizqac.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qgszbfso.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qgnqotem.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jjojwnkq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ousjtdyo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2brapiwjb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gdbxxflh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qufuhxog.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hdqtfoxs.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2scdrcrrv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2knwmzzkw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2vhxayspy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2niudnrsv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2zzqcibfe.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kfcishtd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2posnbkdr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2atetxruz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2aidpohms.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fqtvfyho.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2quaqoefe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2jnqpnnew.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2nlpbtzod.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2cuehziwz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2dhdfplbj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2gueekixz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bzeuoctw.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2aiahcfga.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2bugvmwig.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2keribtnw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qdsdrluu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mkdzgkqc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2nbsamfhx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2qidltebt.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2lkfompsa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2cqfsbmvb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2vdriyrkb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2wblxdcsj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2lvmvqhhw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2crlojivd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2erelixyc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2fqkejemt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ivwkrrtn.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2fxzhzyks.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2meeenwbl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2fjswylqw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2xowllurh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ewlsamoa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2stdyfuwm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2vvhzxylh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2nsmbrtir.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2yztomhbz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2edtcypih.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ropmxepm.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2chfpifyr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2azvizunk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jpvuxres.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2axjxpdwr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2gougfsnw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2nhqajqea.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2pnjfconk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2kzghmiqo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2lhtffljg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2hjadhkbf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pyqdxtjj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wvutnayf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kpeqcvas.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sldtjlln.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cnlylhsn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2psajfudp.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2pjwzxcev.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2scqeuzyc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2klpqtcac.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2wdlmdfsy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2efgfeguw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mynmlhkd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ogvyiehg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2vclqvxay.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fyeijwqa.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ootbotjw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2khdcdaxi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2csvborso.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vjfgldmp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uakiilie.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2xpvvtydw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tjutmjrn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2hfsremoh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2buwijqdw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2pyiqyzlo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2attxwfts.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2bwnrdpet.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2unxdwylp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2iinxkdav.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2oscxlnvt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2sdmmmdym.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2mgrcizrr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2raqqozwx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2cmdusozr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2hrmtozmb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2nfegmhlx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2loesozoy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2urafolos.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ybohpiay.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2mhvrxcql.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xygcdfkf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dhymomnq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iyjwhapl.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zxxthbcu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pkjigfue.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sffgqrtp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dhdjvkeh.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zrlaprrs.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2zozdvscr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ljiuqohu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xumcmpvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fksxofjz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2hzrvusxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nyleyjyc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cihlywuv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2mogqwtvb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ilbrunap.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pbohavbj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mrahtbpb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2vvyyotvf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ieptjnrt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2senymmar.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2txohuakq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ozmybktm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2uykayrml.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2whftceul.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yuahgone.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wvurutqh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lfthqojr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2sdiupudc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2enodmvum.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gjgpiczp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2yssbjpsj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2mpltwkpn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uaxnviwf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qwpchdhe.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qqrsbfhs.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xrwypevy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rnyzxaxn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2mldflpfr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2rlmqwpev.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2zdufteou.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jvldorjw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2xsjwapbv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2plicjehi.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uctyikxe.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kxxhivgo.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2crtumhdd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bxddyhmy.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wkimyoiw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2xruooahg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2gdzzjkwg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2xoqxqblf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2heudveld.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ghczbggo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2drlldhqy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2wohubnhy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sntbqsem.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nzwfyfij.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2plbdfzzj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gbbmlctf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rygdgapx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kueuvncd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2osiovnsu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iqtcnwch.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yccetapc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rojthysu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dnwztpqd.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2zwghofnp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2zhmebeua.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eycdiuey.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2milyrkuc.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kdcgxwem.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2evlswvtp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2clcranez.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2jqdsceut.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ujpldblw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2nrkmbgnb.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2seytiday.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2sxhtasii.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ragmalwx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yvtcrpsw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wikonuxm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2lvwnizoq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2orscuzjz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2sjlrmonu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2mrpdfvat.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fgyvgwfk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tujqfogw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pnxqbzwj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wbifmusa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2nodmalxv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2tpraugsy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ozbemlam.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qdlwfwio.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2iyyqfvts.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2guekecdj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ykglhnpy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iykkmjde.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bcoihsaj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kzjhmerf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hxujupit.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yysygfmn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2hezstfgd.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ccupctez.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2owwmehod.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jmwzmgxt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2azylsmsy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2exdlyqyu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2majjoexn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zjmrhjod.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2viywlpur.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wxvirxeh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pmuuymep.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rowroazw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2iogkhjdf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qaguwomm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xgrwdgrp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2dbybcile.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2palcbcxx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2borggvej.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2kwtqigdx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ggwfsnzo.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2pkwhgczc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2igmalajj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ztmtbpqh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2riktbbkj.html


<!-- 参考信息 -->