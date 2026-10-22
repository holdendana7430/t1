代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2kjzcucvo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qswhjwgt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2roznulim.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cssewcmf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qffwvmhd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gfqmtpkt.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ztbkxgqm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2orkazwop.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dfmpwwme.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ffaxufvq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2fbzoknvf.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2qflpvobb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ijqbtjim.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2fdfeknws.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iglbghav.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2bokvrmca.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ogrijgou.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2emacrvee.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2rzauatoo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cbpjfqrw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2fcwsbsjs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ruwxdmli.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2tebubcmm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jnellaci.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2liigmnnp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pxcyenhz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2bxvskzdg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2pzwypvlk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2bzevqzho.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2lgcesvia.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vwqhzwco.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2yetstlbf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2zteaxdtz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2cvhapotn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2vokdlrfq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2rledswfg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2agnboylx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2zadlvljx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2kacyageu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2eejpgwvg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2yrpruqsk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mjlogrrd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2jusyeztg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hvvpidbx.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ikytbrdd.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2hkkvcxbb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pgxefoph.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nkcadtwk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tdtwbyzf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vuywatxa.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2hxqedkiv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2urjygvwu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2fowlxsis.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2brhmamfr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2tnglyhqr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zcvcilmk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2xwntplhx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mjmldtgb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rvzbmlzx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2htcyynnd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2fnroztna.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2bprmnzmh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2okirfhme.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2gkxwkcki.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2rnplrrbz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gvfjykto.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lhzhmpoj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2knofltwb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2swtkksjw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jsrvfyid.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yuymbtcd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2getkebgl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hbotapsc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gfoygtby.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zkjpbleg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2nwwrsyfq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qxjnplhz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2gmfoavem.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2vxzvhtdh.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2fdlcwkoy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2gruscczi.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2bjptyezm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rwoqpavh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ypdmxuti.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xxuejkak.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xlgcwrqg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2cgdrbirb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2bluuzrkv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2lintorll.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2seleckbf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dzjqnbvn.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jagjgpyn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qppcvbzb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2hfhomvlk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2vohretlb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2dvuqyxwr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2hsdoxgvx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2mzrandfq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zdqoizhc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ezbxsfas.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ckeqytaf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2xwraahxm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ruanusnu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2xwdfjpem.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2fcijxlaf.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qfbzdkou.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2kuflaegg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fadtkuhr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2dohjlqjt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ctdzsmul.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vxfurfqd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2lxnoykrp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zlbfgbmc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2hiffdxko.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2vxhvawev.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2xensoosz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2dgjgyedo.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2wzvynkuz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pjscjndi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2cejctfbq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2kszyddvs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pegsxely.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2nidbugmo.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2mqnpqcqd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2unmqawdd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2aynodwfi.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2rqnjpkvo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2yxpqzvjr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wacklyqh.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2monumopb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mspoudwp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ebkrsbwm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ypzvhhwp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uotznipm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rcjdwjtx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2tpmpzqme.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2bahjdimv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2argheuab.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kgmcasvq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2jdrcmaxf.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ilhhbmtw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ypnnlwgf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2rtgdjzmp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ugpdnubm.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2elncabdp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2sozvdfrf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kzurppuv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bxccjnbg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xalttiwa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ehglmzwl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vfeuztlg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2xkchynql.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2gyjjhorz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2lkgiilaz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2faesywhw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dbwqbolw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ukaxjlej.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wwekclrr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2lvbeeinx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2lizezzvv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ctdggluw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2wjahurek.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2uefzuigi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2xgtioqlw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2syupnzwu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qygruzdu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2wudzbjdy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ldezzvki.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2bxpxkyxx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kodbrrvi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pybqaplm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2igpnakgr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2suojmqec.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2abunixit.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hbvzwqpu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lshfpdpm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cridmyom.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2gtsvyjlp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oldtnjtm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vhwnspsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gxnvqpyb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2tibywqct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mirodyen.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vjwhalhg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2uvikmmtr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2jngxuvmy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tagdmcwz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2etqudnol.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hmvozafj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2dquzetap.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2hyamuwur.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2obyzzhyv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cwjhaebu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2kwskkrqw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gbvnqmjg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2llruswcw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2viposnni.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zfrncrjr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ezktbzdn.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ozxtmntc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2iddmhkww.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qapoawip.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2hocnzmgr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2iojdsusq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gzyznpdv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zjpojcaq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2abtgmitu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vswdamfb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zgpwgszt.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2inkasbgx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2qlheetat.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2afyzidhy.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2quppveti.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2chqsroqb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mplblhoj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vzjjqpqs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2dftvmyxm.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yndbmknn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wiudypfa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2mpznnhvs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2usfizmhh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2lgryatjr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wfqfifyc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2zacgcvoj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cdqeshhb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2znbrjtab.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2peqnykoh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bydwaocr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2gyskdegs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lcezqeuf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2izzacvog.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kstiknnk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gaxxegeu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rxaztigt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rfavzfic.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rotxvgii.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2krrqllpn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2txbjjret.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ioucdfrh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kxximpqe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ztcmnkei.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2otjtujai.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ffgdfxgg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2stfxnrsw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2kdutjpoy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2olzarrxj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2bvgpfwbu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2aamukeho.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2lrkvpdxd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qxvdcjzx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2klolbrfp.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gmbqpvcp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ivrhugpk.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sirmurho.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nuiolsxq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2jareugey.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qisjplpa.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2eztdpdxo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wzkxqfjc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xjspycuy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bjcoeawp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2mtpkbapo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2lfpvcvpr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ijqvstds.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2tmpyihsl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sflbchws.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2aqvilpao.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qdpzbomh.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2guvsjnxs.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bbbfeboc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pdnxexbo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2soixkovy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2acuhrrdi.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2uicnkhrb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2izurtpva.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kpohrdut.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2opqyumyy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dzwtpdke.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vpiypcgr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xdqdnkzt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zwnpjxun.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2piefhqqm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rvzpylpv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2uxdumher.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2rdvfcgsb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hlyweulz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xaagglnt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2slgbowfb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2tkybvogw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vrecihds.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2fzfjnouv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2voogeeua.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2oaztlngu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojgsnbwo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yrgacvqe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgglfehh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ffijvmio.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2pjggudrx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2jdhpqsqv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ilzfqgrk.html


<!-- 参考信息 -->