代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3vsbekzph.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3cibyybjc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3oiaydytc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3emquwvow.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3aojlzzan.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vuyvczfe.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3jmbpknjz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ypytykxl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3nfraivxt.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3qtluqfot.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3btpkrlha.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3okxsterb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ifogrnkj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3olpmrkjg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sckshvkn.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ilusrxyh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fibzbznp.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aijgpcrg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3nhpkapsr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nracrsrd.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mvueadym.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3qajiqixi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3qdreeqdc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dqjblaos.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nlolnkpr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3epqkbsdg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ktfvnmrz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3rslgdlvl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dwvbhoot.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jnprmaaq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nvojgfum.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jqjbvetx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3rzafubyh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3uiczriaw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3cqyuppcv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3exfzblgh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3retggpbk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3jhlffupd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3skxkmdlt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ytbbpeyi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3geatzjvy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3viswwozz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ikvzswui.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3assllang.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3kuixbogq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3arfhetwq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ubqfqyao.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3utixfcku.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wseausru.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vqwblkue.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3seczbxdx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dvunxawn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3awqhffre.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3bjutnnsl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3zvzqawnw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3dmgxxldl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rvhifqau.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kllyvlin.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vhzcnaqr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uydrvkmf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3madppxnn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3bxndgqyz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ztixguha.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3szvhmbvj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wzonkbkp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3cmyrfwpz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3osiuuhed.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3udnjyoym.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3htvpbltx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3uxbzlfdf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3crzkbcgv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kgpxfbzy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3hoftqwlv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3aqkaxncg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3xkqnisdy.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hxkwojbe.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3oeipmemz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3omhngves.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3tsjvujud.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3hbyefrig.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3jlvwfgfe.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3aeyaqqmc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mtvlnwlt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lkymnahr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rvlyzthm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ouhdbhof.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ymnlrtrv.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3iebsbmbw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ealpbapb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3hvbpmjoh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3wpmajbmp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zrercsdf.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3jgmrnvze.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ggevtajq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tvmbevvz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3plvhpdpa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3owyjfbfo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ctomsjcd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3eqtowrik.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3pweedaqv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3wrfpdswc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3eswbopoh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3vkrnwvqu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3lxfmeskx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3dofsguns.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3fubyxaxe.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3thvujdsp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3brghdbzr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3qwpuzitx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fcrexceg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3mischwjy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3espgcdgm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hwjegvcd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3wtzlruzj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3zcjhsmou.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3moinszra.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3umimqxhr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3cfqstlkj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3chbjcrux.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yizoaxuh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mpuzfoix.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3iqmucuyo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3cgmgquph.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ttsegeie.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3novowyda.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3zhbxwjnj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3zmogsznt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3hmgeljnj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ajwkxuen.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jimhhxec.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ycgfezhq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pbhodbno.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zgjaepya.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fkghmuyz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhgoviez.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xbosofnh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3pehnnrfe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3zuyguuun.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cqwheprm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3dpbzfdpg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3cftkmnpi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3rpvwtqeu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rjffqxqz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3puspdhnh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3erodelna.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3kggdrwts.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hzdafaxk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gsmedezw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jamdchdb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3osztxhbx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3cieifeue.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3rymmiijb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ipnsbtov.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3zuymbdzx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3hwgssvcx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3irhhkjgr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qkvommgm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cxpuaeog.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3wykbwnmc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3dqspmrcb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ajpyjcaq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3vkywfywa.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3laxjgvwi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3lhqlyxjl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3cuecoeek.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gmssppjv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3gqnurqhl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hbirecsj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3pxqvpsky.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3jnyjfxle.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dnkmlcmp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vpqyulqh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xezdxolj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3epivrycc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3szaxfgxy.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zlxnqfmv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nnqhjjgp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sabsgqnb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3owyikdya.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yajsrdnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rkvqgxwf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3sxrsuwcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ccpadtym.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wgtrabsw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3zbipdnts.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zfjvdjkt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ipyufyxh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xxusxmlz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ghluggsr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3wsxjcgla.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3icuzdnfp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tiddkmbn.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ehkzmbes.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3bvaclvdp.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3pqvqyhgg.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vexyztkv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vdqgtcfo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rgbxguvs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lewkimrm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fogsqlmp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hrvbfvsv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ywbrtqpq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3tbmngzdb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jyilochi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gkoeyeej.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qybcajez.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dlggsneo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qqujtixn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ekxbbzhd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3mhmnlbjz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3peruqsad.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lsdaaibk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3pqmmuebk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3nndbkzkf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dgfuohax.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uszenqbq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3jnjgcphw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rcdhdytk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mpzncnmq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3wzuiedqs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3acbqvoxe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3kainubbi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qxzbxicn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3evxwleua.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3umggopol.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3pafaaxhl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kjtsxrrz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tgjjqqlh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3uhyxfqxc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ugbprnmq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ttaujssd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tgzttuln.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xnshjluq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pceeyfdg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fdyzzvgd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qwqfhpqp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vazbgfwv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kxzerjxu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qiarytlk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xubaezbi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3csqjirpx.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3urprfzci.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3yopcyalp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3dnfqskzq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3scsvlfpt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3gnilpgvx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3npnegtfh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3zqldketr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3nexkcfwt.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cwtnkoiv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yxgoiloq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3piegkfuk.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3dcpxrvxf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mdyiluds.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vkulkkfw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3idvxjjqy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3yohkubaq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zjvieidb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xeenokvj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dheaamay.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vygenslq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3fwwvkmzb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3mgocjjqk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3shfuoswg.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3seuedehr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mfxfhzzn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3gnhffxnu.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nexckzzy.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wyavznli.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pgcezkyf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qtvzrbxd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fxcftqjq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3wjejlbeq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3mdgdmxxw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bmufhbck.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ggcsjnzm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hpyeataj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kzyhxorj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ifwfjpmx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fjtmrlkn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3unljexzf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sgntfabo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hhhnpanp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gaqasrql.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3khdswtzr.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3byjjmfky.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rullzego.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3dkilbrtv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3jlzznpqr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lvniqmms.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3nnlibyyd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qyhvhipi.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3rnibyxub.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3voltbbgw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yuecdfwk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3aoyprrmq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3glimtxta.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3pmfoofmn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3llcjycyu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tgdlpfip.html


<!-- 参考信息 -->