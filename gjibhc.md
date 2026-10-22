代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2focllizq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xmrbooxy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zbpeasfg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rrytapjv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vfmgxbtc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2stilpdkp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2rnzemokf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2olsrdebt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fessrdky.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ukxdeefu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2konubghy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2lvwegipq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2yrizqzbq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2hwkmdzaz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vignjstp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ychhlxne.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ykienayd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aiucipzz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2yfjcrryy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vyszbkgi.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2daewjgli.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2esnvytpt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2shhzfgir.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ymebhqca.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2esotpjsd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mcucygyi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2gkexoefm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2kxxqxbsm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2adkvrkqm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2cfmvvxti.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mveboxzc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uuncgvsu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2fqijsuoh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2kcmqgzqt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2upcptkvs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2zxfvwduc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2pfuqytyr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2oceyndgw.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lujnixsc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2vrmvgast.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2kbkesufp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2arpjbopc.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nmzqcyjs.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rrbtwmyk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2qrlqnxov.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2vqcgbhlw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ngrpybjz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bavskkiq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pqffnzlr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ylbizwqc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2fjgoitcd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uwckkerf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2nbcrfckt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ntwnmfrn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ttyjlcuz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2jadzhqnj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2rhgszywx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2slvmwhvb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2yumlkela.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ovrsrplc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2rvdmwldm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2hdteeusq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2olxwdhjh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ywjusxef.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2qxsvplox.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xnsmzqdx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2euythxls.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kjjfmkgl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2paeheyan.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2uxjmzlpa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ahcfmcil.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wgbwgrwv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ykcsfmcn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tcstkehl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2xhftgztj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2llecxlyw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ozndjtag.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2zpmhlejq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2emfqiuxk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2qirlmqor.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ixashhnm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2onlgcbmn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2obbxislo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qdpqpkyl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wlkhwyip.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yrabpzif.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2djaxddej.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2qlwreizs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2jbedafsp.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ukdmoedn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2neufwuip.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oxrrmkgd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vplliiql.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2dhaglszp.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2knehqiju.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oawkkgcj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zribikrn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2hwwvxyca.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ctkqzrgs.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2gssrepij.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2xmzhyiyv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2pbabqody.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2fbjwuzmm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2zyrltmdu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2zcgrwnwn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2eeicygxb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2jwdxuess.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xinjdyhx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2jeijkpty.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kmzmvyxf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2csduvxdf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2exqwblxb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zuszysvd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2vfotwblp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2tcxbmrun.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2xowfqwde.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2gsxtbxim.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qewnrony.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2bqhzedxy.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sjjulfrb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2dtpmbukp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ajnvnvfn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ydyvbnog.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2bdukmbcr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2pdtuhyvw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2liccniab.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2eyhtcnha.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mhkslvje.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lvazzzxx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2prgoajjb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lmqpiixp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mwbxozir.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2skbmdvlz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wybftztf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qslekwlm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2vchxwgcv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2voyncyaq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jcdlhqvv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2bwbmnrwp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2uwlbrysn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2rdbkztbn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2vhfgejzn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2igutkflb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vyxontcv.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xcaxzsko.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rixrknfp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bbfjitww.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dfjdbimc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hidqcjfb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2zwwgffvg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vmpkohtk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2fnrwydku.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2amblxapu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2rlaxhvnm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2snbigvee.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gesolmxs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2fklnqslk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lbybctmb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fzqmqiiv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2yaxjerqu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2smgwhtof.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2egeizpwf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ovbfokaf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2fcamgmrg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ldfuvmnb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2nkfjisfo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ojvquvwo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cvqipawg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2jntxmgnr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2qlpcxcxl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dydkuxfc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2irbgehox.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qwwjpivf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bpwggkzl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kgynypkc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vunzkdra.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fjeshhud.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nfonxvii.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kymfgsjj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zrfnwxhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdsddwto.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2dystuwem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ayjnyejd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cvzmfiwo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2rcsafqqh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bulotoxh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dxwcyjuu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xfytuvxq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2qqcqxjpi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2sshbykks.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2eofqbkpp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tpuvjbok.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2glgpbyuk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2scamzhhk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iiyscwmy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wytzuszk.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rnwbhxfc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wvatqmpw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lzknmzpe.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tddjgfjf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cpyaxymt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fmnkezhj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ogvslsfr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2katrftpi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2chwwwcgt.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zopzdmey.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ejyjbrts.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pguvapqp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2cnvnzrtg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2hqoujgum.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2sbdiypix.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jyggncdu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2kavjvxlc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ktqefmmu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vrcwxgnz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zohfvpkf.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2nszuqkqn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2blplexli.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2sagjejec.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2vjlkvhvy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hcfevsku.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2lntxrcjn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2siyetslm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uugutibn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wgalvjfk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2xmpnrflh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2icribpgi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bdjmxxnp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2bqlgnsqw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eghufboh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yzyavjhi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aluqruok.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gmmwmlho.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ynfaghvs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uinvbpxi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eczlqand.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pchvtllr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cnfrgogg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2xjclvtwe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zbsvwywg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2otvjdsze.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2mupgtsrr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2cvawdwys.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2umdayumh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2mtronabd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2nuyfscvr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2uhfaefcb.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2vvtvretb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2xfssidfd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fedutisb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wptouxwo.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2euveeijq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2txogezzu.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zrnhmrit.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gmzeadbt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2jpvahptq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2fgrokwtn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zgbucjvm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2emeznsdr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lfqxcmxv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2bueijqsa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2jpraqcma.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vbptrnqr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kebyrewf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2pbjxqjex.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nfvrqjnp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2sfgvciov.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yztxvxoz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2azvsnike.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rzqdlhqe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ekhirjgf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2scarsykb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2whkgxjrm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2twwyjmmp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2blwxtxrc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jkzwlhfe.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rmpaxcwj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qpwtfpju.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2naibkucy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hoffopur.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rlgrlndq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2schnhoxu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2lnrsriqi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hemuubza.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2xxpytjxn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2utupmbtt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wsjhmhwk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2geovpdwf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2utjmwoib.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2eaowppmg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2dlyvbovp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2zlxebtfl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2mygugnkh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2iitqrzwy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2skhzuefm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2whukfbtq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zfjvmgdl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kfjyfzba.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2hjsheakn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2maobkizf.html


<!-- 参考信息 -->