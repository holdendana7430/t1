代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2dymkkfgy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2evnwkrzj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kwziapdu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jtxjvejn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qjcksfoy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lnwqwoid.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2mznpgqpr.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2zxofrttj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2oqrvuxro.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2dlhwhtel.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gavpqhkz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2xhmenuap.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2khtmsety.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2njfwnguz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2zruvrkbt.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2dfswkpqq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xbdvlbdl.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aqwphwci.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ozeuccfx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kyubcbso.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ndlkjpjo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2fvkyynio.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2sbteldck.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2exwqvndc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xwrgueka.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2tfyubqxy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2brsxtwbt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2dlskqiwj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2kxjpmfys.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bhrzkuse.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2apyslauw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mckarshu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2sxglnkxq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2feodstxe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ufhidxzr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2oncnhxgn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2gmpquwmp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ctxdxmks.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ioslcywm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2zslvxwix.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vhrfjxtb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hwaknlcs.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jmjpiooa.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vyjvvxcq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ttmuaobb.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2pfeovyoy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rvwhepwy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hzwbvjkk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2efvgehld.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2feqtazhn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2raxarhkf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2osydsjgf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2mjscaxtr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2oqcwupzo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2yiyxsrly.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ddzahvvw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2slfpqcjf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wbiwipep.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eoanfikn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2fmjpvbzk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2hiyrkjbu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ldxfhxev.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dofbsxvz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2eydwoqqh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ehtptdch.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ikznhcev.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lcnurolg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xphsasco.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2pubqgaiq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vofiduje.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xicgmerk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xvmibhqy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vqmpdkbs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bzkotmup.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rpzsodjv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kdqzogoc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xuoudlqw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2bdjuigkb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2jbumqqsp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2vnxgwefg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2yohozwlp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2aznyrztg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gqbdxvhf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vzleumac.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vbpjsaiv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kmkpcmof.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2iftwisxp.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2obwxurzw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2hvxhmejl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2akfijpdg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2deoiqfwc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iaafipds.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vicmgkvb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2eavoajwy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zzxgcftw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nfgxpldh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uiyffkiq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2iixqvsgl.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2uxaihcsj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2uktxikgs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ssaztqry.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2jpfpogqu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2jrytiigu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2jhucuwcm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xpsljveb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2oknayqev.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2tvtqjrsx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zvlgohxl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2mradweov.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2stkvmqcs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2hcanzwru.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2clmyqrua.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zemjezqk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2fwkjixmp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ybdfkqpu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ocyjubyn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2kagescyy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zrvzcytd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qtbzlyum.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vsxuokqs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2myexascg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dhtuqbqm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2bcgdoadk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2stscjfhx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2schlkmxx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ojhobnah.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2nacjwsic.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2hkcukplw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2lsiqqeyp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bjzbwmcf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hditobbf.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2snabaxyg.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fkvnqbxz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kflfizft.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2myytkzlf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ldzecyyn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cbcqwcsj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ucpaojtb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2hylwokml.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2qmtfbqhp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gehmejhs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2rsaklqhp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2yzlhsdie.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2tecosoue.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2pdiuhiaq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xyqbkpyv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2bcabykeo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fkumywqa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bvzoimrz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2enrtlepv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2hxialqdm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2pourmdom.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2pdlzgfon.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ahyzxxtu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2srvhmcda.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2fpowveiq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sxbwqmrg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nuoqhdzz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2urcrbkny.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2httfyguu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xrxtneyd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2jzqhitgx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2yrksucht.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2qirvhbbr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dzbiuqgy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2rjlkttqh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2oqfiwggf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dtuoklps.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2sqxbrdlx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2marhsdaj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2nqkloyvj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2trhknumk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2tyyvhxfl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dqtgepce.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wwljkcrt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qsprtcqu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2azpckdxy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2cpnayvxw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2equjfnjr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gauguwmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjphpbta.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ueztytas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqfkpeiz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xcetwduf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2gnjayyxo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2iayccpyy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rehnwxen.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rskrydts.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2nkdbnrvn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2odyopgzt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2pmxfbfuw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nfjotwpg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2wribuubd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pnojgvcx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ggbqnddy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wrzrjykd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jdgxmhwi.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kjpemovm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kgnrtnyv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cyvaqcfy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2sitvbtdl.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mynvyxrt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2fheubxhy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2adwagkwt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2inetkcux.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hgojscmi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wdlwwebu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2whgybinf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2gcnqebrs.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2uaneyhef.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2wvpiyyln.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2maeixgfs.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ynodtzww.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2yjquiarm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qjzggocc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ztajtapl.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2clwfvhka.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kfxmvuzt.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2aicmlhvv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ewsgbgpc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xqhweqpe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jrpwqlzh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2padslnwg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wmxqnsqk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cyfymedi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2buqhwpeu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2aakreihg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rizmvpkk.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2vrsiahxs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2esmxzzmo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2irgvpiti.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ssavhzix.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2effmidci.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lewwrymt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mfiufkxe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hjzgztvy.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ipjdbstb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rsnmlefj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2keoqorbm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ckyxtgdh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wkbuxmcq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zazokqya.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2iyeqlevy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2mkmyqtma.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2gyfssngj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2becupuuo.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2fzwfeugy.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2hprgsxgf.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2uxbenlym.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ltfvurhq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gyfzizds.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cpwewfkf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2qtujknyt.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hdudbbpd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jnaltvaw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2rbgimzbh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2cysbwvpc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hxxktvic.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qmwlkzdr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kpizhwvi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2unaypvaq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2lpfxfjbb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2tiicossw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2etbzdgce.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2wlopvaki.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nvumtmvb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2qsbmiwum.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qwqlnlgs.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dmpnudms.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pmmvyxeh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2csfforia.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xuvhlpvi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2lbxtooci.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zrijnaew.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fkrglgtz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kpcqurhb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jxxjkdct.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ctmsoocc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2elenkwcy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wvfkknmh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ovrvvzpn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2tbhqqaov.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2operfqcj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2htpqzwqr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2cgdckjar.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fynognjd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wyuwegwf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2cgwjyxwr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2zmsprfuf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fcwhiekf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2laueflss.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rpkucrfr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2tmgxyjpn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjihfglc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2twytuqcg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ekphdkvv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qjzijkli.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ohwaksrq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2nnndgrdr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yqxyivdz.html


<!-- 参考信息 -->