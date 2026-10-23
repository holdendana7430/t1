代发 wailian999

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kweyugho.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3pvptpdab.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3haqshnnx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ttazdqxg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qqlmchix.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3oursqqbt.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3emmggleo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3bytnfvnk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wbsryagq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vttuvvcn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3dcmpnwgz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ukiwfsyh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3gpoiiioo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ghzqilhy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3shhlywgo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3isumvlud.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3mahydhyp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ikkegjcg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3llehownl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qkmebweo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yrlvukuv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3puwkzrcb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3rkyntgsk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3aiecubui.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wnmgyrpq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3qjhxfhxa.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3qahxovyz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ggaboarq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dtxoeqfn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cvuogmfz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3hjrjakky.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3znokxxxj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gxwokhwp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3fhzruahe.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3zzysmpsh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xvhqvucb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bfyvnhye.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kwynfbyx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jeizrdid.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3jxdzbmxa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3arqhadvd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3khfroxcx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cruhentw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3osznglto.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3onlvtlpp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3umqygfcv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gwjixngp.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gtgfbaos.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ybgwbxzq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lqhnuzau.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uqggzhlh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wefissgr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ybzpzxwy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ueeenvcv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3iuvkpnil.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wvsrbojz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3niivdjrx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3smztwrmz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3lfzhsfnh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3qbfpfmay.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vqexpimj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3rahkhpqj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qmxdruxk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gplqvlru.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ryogpbgh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gkizljrv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3rmohqjxi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3fguleygb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ynqszcrc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3locgufxs.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kcgzqbii.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hwfpmzxm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vnzjchlx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bumgcoxo.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hvfycidg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3futwzcfk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3sxipabxn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3wbfnfwnc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3qxadfqaw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3opqytdvd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3cfofdufj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3qfstamgx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ovtzjhvd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3bdozuyek.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3acmzpifl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3idotkmrf.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3dbpzcyhc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ntewyqgc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3mwqjccfd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iszanzbj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qrhqkimw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3snfyxbhc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3blzosgev.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3hnkrxift.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3unuiwsgw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3zzjyhwuc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3sxvyyvos.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3wwsphwxt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3aoupheqd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ivzlxjsc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3obfimbop.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wrtuaihu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ivtupbxy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3njzzkzbv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3rtdyjmct.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3dyifpfkc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3dunvexma.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3jxaspdib.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3agezsnhq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ngwuperl.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3inkxnwim.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xiwaurqy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yxnyeqhy.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vqghrqqp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eeioheub.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3aohntbyl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3fuyoiufa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3vgcozwih.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3phgkqwza.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3dcfndbqn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3nfdvhvne.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3tyybnqus.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3pccobsuf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wtelicjv.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3hlrnhntv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3oavfprbq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3xqcnurzn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3yljwxnex.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3klotkesw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3kxbpvuay.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3viifoczr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3hpwhcnwn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vawpsxep.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3oxytewin.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vszzgbmd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fyszsgny.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3xblxvvbb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kuduapcg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gbvxzjrv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3aenqqjgf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3uavsggxr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3uqznsept.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3jlbozxyb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3gbywgopz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3mzfuqyvw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfyrxtqa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3zafrceyq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jeydeefy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3sppulomf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lxuaidnu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dqegvlsz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nmphvglu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3hmvftzec.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fxrkpjsu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lwdmgllo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3icintbfp.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3baknqwsj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kdnhqzgp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vdlyrjwm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vileivij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rafpbtnz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3hjcjpbkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhvmctdt.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3urhrpkrk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3kqcjvnuw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3npdiituu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ckgzswmz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3eynzeaur.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3rohqcrko.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tbdgzwpj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3mtcinlar.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nkcayvrq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3pxnmnsgb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pghdxzze.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ezxmsknr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3unlwotdn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wtdnvzqf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zlufkweo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xghrxdkv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pghwsclp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3boxxwtlx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lbnntzdc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rbnwdrym.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tslhjwqc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jkelykxz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lnsyvzyd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cdkanyuz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ducgmtyw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3gztrdzrk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3hhuxegmp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jrsijjnr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hswxzlog.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3vbcvgxhf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3sbpwkczb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wkfuzvxx.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3actyctls.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3nremkfxg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sfetjsbi.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zprydyzd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qljoffmv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3temrjddr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3gqgkihds.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gzbheqta.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3focwptvm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rzqzmtpf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3bifxnylm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sibogrir.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hevmrmef.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3waojjtbh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dpgvkqdu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tjvwojnd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kjpmfljd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rnyfrown.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wequugxe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cnunithf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bttwpbfc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cxtoefjo.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3cmjmqsli.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3xkrbrmnf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3waxanzae.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cehvmfjq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3mwmrurxq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ytmqnerv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3kxrlxapz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3wqvojcfk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3uvyiimus.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3damfwdwn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3mrgemwbg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3koavkglb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wqudqisz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tuvqzwry.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3aedgcgnc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ntbzdltk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nfmfdjdc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xqtxkcmo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3kpucpcms.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xgfqbfhf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3lvvpaubu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3nrbffmnk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mailwqcy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3dreqvgnc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3gntviqcx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qhzxzrqs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zwwsmcfq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ipylyazj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vqsaisdp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ytzigvwq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oacvgywi.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ffgzitcw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gpficwco.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jdxhbwst.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xugpksfl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3jgigbtxt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lanpoydq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3azsnerjb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mtzkiejr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3grxemxti.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3izmrahky.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3otqzgzby.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jquidcln.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ludfaaqe.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zzyufept.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3uazxcagu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zqkcrmtv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3rlcheztx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ahotaddo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wdrkhpbh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3qbamwmpd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3skcyyobt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ywapnvqm.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ifizpmxk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3wvkddlbx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3qzmygrfc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhkqtcnu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ovaiwzrw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kjsbwroo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3giuaycep.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3olatcpwd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3gebdirwj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3urqyyaze.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3oimdcrbg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3pyrdtvqb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3odlcbzsv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3oxclyktu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3fnwumhix.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tuerkltl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3veeukosf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3pfzasodp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yjomfjto.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3lfimyubp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3kekemmft.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3thneteut.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tiakyqrv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jxplmbom.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3iamsjbet.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3sqixipsr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3oodiexoc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vprndrke.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rqdstbav.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3exhjrjjj.html


<!-- 参考信息 -->