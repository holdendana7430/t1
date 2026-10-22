代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yzamtcmq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dmmblmmm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2xvgclyrf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2gqwlponv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ivxwzjgt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rfkgvmvh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gcyememc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jmnaojtl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aypkfsea.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xqtdqkpd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wadvarnb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jepgqdmp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2khusyycg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xypuxodc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rqttqwik.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ojybgphc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2tqxruuvo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2gizbujtp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2znwffytw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vwtswllg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2heyblhtn.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2udbnbdib.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2kanzqkxg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2yzxwpvty.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pvmdacin.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ewdkvatx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ihjxorbg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jvctzpfq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ojbuepvl.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2jponepiz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2szchybrk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2whlpdkkn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nojsufob.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2abatmrex.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2sljdwxui.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2alpqydce.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2zwwjmcxn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2qrzogvpu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ktcgglvd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ztnhzcuz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2effduivg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fuhlxzpt.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2hlepcsxm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2cyvwrefi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mhsgdzjs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vhfusmhx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2axchlvlc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2humwngjh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2poksffrq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2cvjourmp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2exqzohgc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2mbovcila.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2hmfrrejm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2dorsiwrn.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2hxkprdol.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2lugmnwjs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fjmisqnf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pqmayben.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2pezuukos.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ahmwsfvq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fcunqqbe.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2fkelfhfb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2bqdiackr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2akvgwkaq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2czrmssub.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oojxpznp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ksomcnca.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dumcviln.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xvuffbkw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2lckdadkc.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2uykszawh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2qczfrvtq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2qvbtsarq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tbiandka.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hgyfjlsb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jyrcpems.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2bkquiupc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2smlbcrpq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zcgzzetj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2pjaluivl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vfxjwphw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mgqavlkn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hzzgdsqd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2nskazvwq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dofaoqkz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2npfwjyhk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jzcrzgnc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xdragamw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2oafyqyot.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2agugjiae.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2xqddhgxr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jclnegdg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ibohimvs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2tklgmntq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ctitdmun.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2bcqotaxs.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jejlmfmu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2sjdhhguk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lzywbqmq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yfdwwias.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lrhrwmrx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uboigqnv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2zxwpdpdh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2aqvcgroz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2infrxksu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2wudjvvlo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vkjwnolm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2adcwykuu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2drwogigb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2pmjuhrjb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2levklmnk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fhueeccn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2goobjscj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2llizdrbh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2lxreovng.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2aonphykp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2njtmfgxs.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2jxeiodsp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2otbfhbrs.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2tqevltna.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ovwnbvge.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2umszjygr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2vfvetzhp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aanjyfeo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2dgmatwfu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2puwgoofb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ngyjieii.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2eszemgye.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ajytxusv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2aiyxflfi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2srmxbwfj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2zuvqckpd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2axwaysyy.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2gzxdfhmr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rcawzsxw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2dawveita.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xpnaasmg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2getznkix.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2pebsfzds.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2vucbqqyx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2sfvywmpc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2gqszxeyi.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2wlsbgwfg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2hzjjkpek.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ihegnkrt.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dxcvwrzd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cutzkdtp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gvufvrfv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ribvqhwa.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jnetrixx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hdbpnfcj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2olkpwzdp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ntqjitho.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2bnkyvykz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dzwojiwp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2okpnlppe.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xdgyuxmg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2bkohcgyg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2myoevgvv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2icitmtrp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2caqwseaw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2moolldqk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2waytxawd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2tckmhvvd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iniekhyf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2mrvlexdg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mesnvajq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2aagsaqjg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2xvminrzc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2isthqtap.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vltnpfwq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ldretklh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2irzsxrda.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gzdckhzj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bwbsxlns.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2yrzugrpg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2hfztbdwf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2bkmrkaup.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2rbgqfrji.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2uwywhlru.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dcfngvye.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kzubljfu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2brhpcvgs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uihthxuw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2spxtxbpr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lgwjdetq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2phtcyezo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2kgcvfkms.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ponpmkrv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2edwuroop.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2oztgqwed.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kornpgqf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xsjadzzb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ccienfgi.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zmtcqfqa.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zgnrnxjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfadqtlc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2mdzemwma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2stawkraz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mxbaqzwz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2cqulhomu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kupddzfw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2woxicmcb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vemdcvoa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2bprbhuko.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mxnxooim.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2qlrarjlo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ddhahxqm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2byzbvqip.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2yzlmhubt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2noettols.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hbluviqs.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2snttpegh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oatoqmqx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2uhufwtqh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jbeuzdeb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2mhsxkdrn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fzaolgjr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2pheilqbq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rdxjdmtn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aginjrnw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2egqyvwlq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2uffqknsx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2iglkhxac.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2vjltqdwn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2cqdmxgrs.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2uyraqeer.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tcvjscaq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2fvkrehmh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2hbjugymk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yaliiewr.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ownhfzby.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2caquzjum.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xagrhnhn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xzamkwql.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bekvfoqc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2zaizsmgs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2fqutbqef.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dqxtjpvu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vznysnmk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hbhhynau.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2knvdqgfm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jnzlwizn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dgjfoluw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2hakvargm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gfiximlx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2kywkwfsl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cvjurqwj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vtabfgwe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tvppsgph.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vomkrmdh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pwjwwhyd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uucgpjqp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rgasqkrp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2xjzlpskc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vrcyaxfk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2zkqbgsik.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jqtqzflt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ldwakrqr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2abomlrbt.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2htelhqge.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2sxomlqbn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ovsbuaoi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2codxsfav.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2bxabkgxe.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2abrbgkuz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uerzjvaz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zdajdwnt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2tpuwxqum.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hhunjrst.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jisdsimb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ooxrkqkk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2aakmenrp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2knzptlbg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hejwkoaj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2krjxmkzu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xdpnsdmp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2xpsurcbh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ckqgjmxr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ykvpesny.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2emjwgdvz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iimffkno.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2jputvbhw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ycvpgzvf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dxycjlba.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kftkwdwk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rqyxysif.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xithnnzi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2grrrppuy.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ntqlyxmn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2miuqyotd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jkojppkk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nmsfzpkg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jetbijbs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2vjluyokn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qxdhvyji.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yqrgjhrw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2uiuztwdm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gfvxmnkv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xgjfzlrq.html


<!-- 参考信息 -->