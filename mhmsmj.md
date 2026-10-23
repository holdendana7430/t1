代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xaijosdg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lnliybjg.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qbuqiksp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3rfsioiri.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tbcwdguj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3nychftgl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qjozisza.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3qlhumyfq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3mpgtgbij.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3wdpdjraf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gavzbufz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3xwuqzryx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3gnovhdui.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qjllqwbh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3coroomsi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3neodyffx.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3teyubwzz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3tlitxfli.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3hvfajrmu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mhbplara.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jhoeouto.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jbendbvc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3uwxcldei.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3rbumucml.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fkhoguct.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vcnidgnp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vvmwxkgb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3auvpxwgv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3kigyhrhm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3hxlflvwo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3upswhsal.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3euhvaiij.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ojwaicjx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3kbjowprc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3gpgtuuko.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3fmwxexdp.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3thtjjauq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ytftsuxh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vqhcmpjt.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3vmwgepuk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3uxkacovh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3yhrqslnd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jtwdtjfd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gqyttoli.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rjkmlitx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kqidcjth.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ovhrgkjo.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ittridgj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kegbphsq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3hnnpunfl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3srnsgzrg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bvixtpef.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tjfrcfko.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qbarmeti.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tvknzjhy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3wiyynbqb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3gbnbquao.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3jterdfsl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iiirtspp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3sshptjmt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mwxkuqxj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uirdkbcs.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fesabxvb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hvxzbluk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3pzctssfn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xybzpdkb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3urxshflq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mtcoypbb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3vpdqfwng.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ijvjbcmv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eejooplq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jwybwliy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pzugpmww.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3evihrzyp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ivxjzkkh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3cfqpmexq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3lksphcvo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3shruxlhh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yfaxnlas.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3khbdgfik.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kekjkbdi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wvyymsbt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3qbspzsll.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ttaoartd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3onoxzinl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3dqxutlkn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hkjqmtrf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xcbwfvid.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3kohcftae.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3udbjawql.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3medxymtg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3btecakfm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zekdjxqp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3kncbhkqj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ipevhmnc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3aghqwvyo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3lavmzdlc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3owbakgex.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3pbadbyix.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3cmittvln.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xfordjva.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cmzgvsie.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3lveqwdlr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3klsnegog.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3timhkibj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hpsxilol.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qehkmetu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qnpnttdz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xpfxeimu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3mspsmawx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3sflyemci.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ismpycgb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3zepgniza.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ybsmuocr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wryktcbz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3jwmlcsdo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3elydohls.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gncqfqli.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3vswujnbw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3gxykuddz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3yoorpzol.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zpfxopaf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3lbzwcfkf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3lnzjlnne.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3gxlydvpd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3oxghqdsa.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3swbjwrnh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3arjncpjl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hjtckgry.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3aicpujwj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ewwaspuf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3dwtklhik.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qzkufigo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3nfyglpoj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wfvxebjj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ywcragil.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3hjkvwrdl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3uoybibbm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3wrssgwwi.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vzxsyyfj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3umgqtvhw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wntmfpfr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3jylaahor.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wchuuzch.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ysvgczng.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ozinruqm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xpjkuzcz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3xanzmsne.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3vnmnphes.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3pcgfkofy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zdzoupgs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3psgpbnym.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3jelgvkch.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wpxskmiv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ouecqweu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3yziammfp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3omexswgi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3nipbpnvj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3icabonou.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3aivzffpk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3crgaplpf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ewalrdcn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3etexbvpv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ptbzjylo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3tkgvnfsx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bxdbcknf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bmhgfurl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3xozdldxm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3keyqiafr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fbqwcomg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rrefksyc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3caulqque.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jffjqmoq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fftyqnkj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kktyuduh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gghqolcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvmpfffv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3pqtzjxah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jhkqfpdm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sjyvrvud.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3qykstszh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3nscpqkis.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3gswttkxv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3nzuxtnht.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3thpqymoz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3egwjtipj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3wbltwdxe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3quuurrqk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fxlmlazt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fyrdjcec.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3upzclike.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ncglyzcd.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3juznskyh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3meeihzwh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3elsmnkmd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jjlwfygs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3gxfnmuis.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gxkucssg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3nfffjpnj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cyrqjuuk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3piclfagb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xizliqtd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gvjbyspv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jjxmgdba.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3lcjagjhh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bfiyuaiz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3olsdwizu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kyqegzbo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3waexyzpx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3qxxrjevd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pwksuhgp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cesmamlr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3hxyvxnpq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ycsonnqj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rnrvjlda.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3bexyssui.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ufvhfpqh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xkbwlipv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3skamycfu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lusjbueh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3icdvcydk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3aqpodkxd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3eobbmneu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pganipfp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3sbklzmzi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pqdfvbpe.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3vvfsrxzs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rxctzzqy.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qpylqlnc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hcblamrv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3exqmpysb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pquvxqyh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tiwnfdlj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3yzfanqjy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3aakumuzz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tyllljma.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3qgskzrsb.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wfxapuna.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3yejfcgbe.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lsvzbmis.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3cvqqgovr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3lwoaqebc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3uticmygj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3pwrruqmm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3fmggaxep.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jlwavhnr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nhpopnge.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3buzahtxi.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3fpkztmip.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nwreusbn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hauhchmm.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3pqwifdux.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3smhttwya.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fzuucvmd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ngamiiwu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gclfdpoa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3idyqpkvz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ffnflbbw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hxfdlzmu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3fafgtivn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3tnpnrpmk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3efoaezgi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3saqftyqg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3raggtwhz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pizonyzq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jftljlul.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vgdivkfd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ctehqyce.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ktxjsxan.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3kzxbepex.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wrvawycb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3apkpthsx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rxbkckhw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xlyhesrm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3thylxrhy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mpfhfpgy.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hfhtjylb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3htamrmul.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3stxswaui.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gkynbgmp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3mynlmneb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3agudsptw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vacjcuoq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3hxodveio.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3qxkspxrt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3uamcwovl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3cnjgnzvp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qwybfwuy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3awzyjobx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3jiqcssoj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezuybzcx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yeckblfg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qvuwqcch.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3brvblowg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3fltixqxo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxirtdwv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ihpinflg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3mrghatwp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hdowojqd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3upkbindh.html


<!-- 参考信息 -->