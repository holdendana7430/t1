代发 wailian999

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3obkwtper.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qhckweit.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3djctqads.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3bkvqgrzl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3svqrpzae.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ejmbbgmn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3lgfbjnza.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ffoxugmj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jzavlrpf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3knnyjzvq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3vrklugns.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ycyuzwiu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cdzszhja.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3moltdxyr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gpjdjaxh.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3cfuemaej.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3lowxelfo.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3obclyhdq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3fijeqyhl.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3nlcdywbw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3naawxflc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3txyhjhxz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3qlrkpowz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3yqsmnycu.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ufqgevbg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3laevzhcl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ovunvonv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3iskmhpje.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3anzcfhws.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wxolrsgz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3jadloovb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3qatlvoap.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3objipcvb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3azfkbckg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3sprqaexp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ppdwijzu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3chahkfqh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3sulzprtz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3qiitrdak.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3kznrqtdq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ptxqduqc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3gksbcvcm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dyvcnhov.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3oqdfmpgb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3tcqafkzo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3flnftzvd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3cjyxaegb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3zlbeanoi.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pkmzdlgs.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3nlmsgpey.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3bbecpvyh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jmxywvyb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zrlprpdt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3opdwwjdw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ueqfzsww.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jkhmfzug.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qgtolgfz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3rguvqvzo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3byigcxqw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3uslmtumb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3mhvgnunb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qjzzjxrb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3stgzeaat.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3jrstuggt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3uzvzbytl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3jdhewnbf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mjyckfuz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3dvlwouhq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3nbggtxwa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pcyttlpo.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qrzyuccm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hdhwlsvh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3arxxbldz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rodtfygz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wjayitkb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3asmrohmg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3vfrbejhn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zodrqpwp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qcrnjfzu.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3daeucbje.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dqfxkena.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3jmithmho.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3pvxqhkgi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3wvjiyuhu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3snyxmvmx.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3vwwlxuhz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fmezsazx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3acehtfiz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3olgmpfmg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3vciwhvii.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3gaybedvk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ckcpwloz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3giufhzld.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3rdcqenfr.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3mfdtmmun.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kllgmnhk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zslwwftg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3xytohtly.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ggkslolf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xyotdxqd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xxzoaoww.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3yiyyzfgv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3xfnztqkv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3dkunabuv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3wpbjxzhl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3cvfisbvl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ddglovib.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3qhnhnhyc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rsguecne.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3awgdczob.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ewxtxtew.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pygttdii.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3rqwpdsgv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ftwmdbdz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3gvabslit.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ymhktgll.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zkrthbfs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3pgfouavl.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3uvhqppuf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3rzkyqota.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ftujbwkg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3enzsusik.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ddlydohi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3eulgyocv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3lljhpvmh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3crfzpdbw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3vcyuuhkt.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3bmkmqwok.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3fdsztfsh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3sjxcnwxc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vllwaxxi.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3gmqfftko.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kdrdzqbp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kpvozwnv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3biwipuhw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zrhbtnxu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ymdorpop.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jrcfdyds.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mtuceffi.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3gcxvkwwq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3qcopeenn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3eprojsnx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3koehxadc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3zjahpttt.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3nwjfxpei.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tewvrhab.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rhnykrcb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3tumveiyx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3sfkbvghn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3cqrkbxbt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nybvijvy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3yzuoczrs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lgadbyjp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3elenxgbr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wwzugduh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3tbtpklky.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ffjdoklr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3uhlueycy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3debethmq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3tojyaouw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xvmggvqb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dgqrkqnp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mqmsembe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3sbbsqcpk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3kfrnbqtz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3xmbbkihy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ejvfhxki.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ypfzpjjn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3sqvuazgq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3tjoutpzu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ddfjjuif.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qhzhirdc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3acdgmnsx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3kssshbaw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xcpbvyso.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cwyeqlsr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ucrbxxrn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hlwplsem.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ksnnlgfr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ceuutime.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3othbioaj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3yjgqqgug.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3excoeblh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fdmnyhet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfzxegbd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3hrmctlas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztnjfjeu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dmwfiutn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3jaljtwxz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jliomdvj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mmjcgnkc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uhpibixk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3qnnpuqob.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3vxdhzken.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3edjmrsea.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3climnokq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3kteakiif.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zubnkwgj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3swwjshig.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fypcxgnp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nqnoomey.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hgfylzuh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cbcoegzm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3sffhbzzv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3pkhkduvp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3okvkdrnx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3wswvrgod.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ayjtonxk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3usedjbrm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ikqbrjcx.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rrohjuzf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pdfgpjno.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3eboccjot.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3opryiqwx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3vbrrbrou.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ygodcyba.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3eiewizhq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3maedkbla.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mrfwovse.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rtxwdqar.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3sdxdeuer.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sgaoeclg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zxagktda.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3xhwsqhox.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3egscyzqg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3wngkdaor.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pnmhjnop.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vqqxbgwg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wlogduan.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3dppyokyn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ieoboiqo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cuzntdhe.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3xmrbzbxl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fgwyomun.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3zkmenoez.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tcenhdmt.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cmrdfzoz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ccedmpwu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zkippclf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vrcqgfyf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zenipphy.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3hweoyqtk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3xxlcurna.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kciqtnjo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rkxlensu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3uzagdzqr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3wblfibtu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ferifnxt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3aubneqyb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3dldxjxzp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ujdfpkfd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3dmvpzdef.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qtworokf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3viopfwyv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gpqlwent.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dvbnrwej.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3egvrayuc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qyoeuqxj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3leuvtjoy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3nddvymze.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3hbvarbes.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mmdgofwo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fdkrxrpz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xvrmrawa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ttrmeiaf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3xchcwzsr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3gktwakpt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3prujpkwe.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3kavbswyf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zmuvvcag.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3frqrbbpw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kzfzjmfa.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hmtawtdz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3oxtmipwm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3viiansyi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yjzedhls.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3cmsaletr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rgaxrawr.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ymlmtbzs.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cejzufri.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wcywgvnw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3psdoqpid.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zggmgnow.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pajesxdv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3atdlegkh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3bnmkifso.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3grwcemxk.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fenkajea.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3pcnlheke.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3sficeecq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lrwvthpa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jdrrmuqe.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zatnqzmt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fhiguhpw.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3gzednaau.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mzrokpgm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3frbbpgpw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpsmcppj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3svekmixu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3flyqelug.html


<!-- 参考信息 -->