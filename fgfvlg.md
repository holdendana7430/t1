代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ihiihwfd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jjefqqhu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ofdqxmcb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xdvkipxc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2iwrooahr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2uhuhddpd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2unhbhcem.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2qohpsver.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xrlemdte.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2szxgdtwl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ictkafba.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ejefywsv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2bhyjnvas.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ekbtdzri.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gpdmttqw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2herskojk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2snogtvoy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ndootgdd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2qdczmpea.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2lnycjrew.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2lhxhjuus.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2smoxjnfa.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2skrpgmdx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2iodwlkxv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sfganabk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fnmfuxbu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2kdpovwig.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rbvywkuu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2etyyigud.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2nmkqnpfp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2axrhbltc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pokolynp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dhviimtg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sfbveqic.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2vufteegm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bksgddft.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wycpnjqg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2tswtwxok.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ofnzkqgs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2bmyqnqvh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2uvvwauye.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2arvgpxcz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2opgaseab.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ejcpofbe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jvicqqzy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2gouukxld.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ayqwaurc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2evwbuwuy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2njqgpifo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kyfsfyrk.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zfdgmbwz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pdxeemty.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2cnpvazto.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tbyznegg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bjdcyoqh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2avcpwgaz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2sztukivy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wsrlnyum.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xdoidxtn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uzmqfyxv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fsthzpum.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2rhjvzkzj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2opwsamop.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2fnfnixdc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2nidnxqmc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2nokqupji.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fvyspmny.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dlqkzgyn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yrmsgqoh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qvorsylh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2skwzidoj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ldkpyqhf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kdiwbxet.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2xijmboar.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2srzqfzmq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2katnxoxc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lvfnlpan.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2msdavikt.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gqsfuwml.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2nvegyegg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uaxegqkp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2fwoymeti.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2lzyosaux.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2hckpzipa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vrmewbne.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2bxidjvjr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2lqyqylhd.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2urnklmke.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qgqbkhro.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2uxdthqiv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2kxhcmpsb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2idfwtgty.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2eeqfhoax.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2isdpzlxm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2chyrojjx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ftduhjrf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2szgrjilb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2febmkyus.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2dohwuxbf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2hfawgpfz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2sbwyzljv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2heddbpqu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2uczizfpo.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ijqjoqqv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bmqvmkng.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2kjbhcosb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2zrhhbkqq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2cbluuzvk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2nukfnaji.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ulbobdqz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2itlyvipp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2vyirrmlf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fwonzvgh.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kmgwdoal.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sruffuua.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qmjdhjad.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2smobpnhb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rrtpvcrb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dmhnubug.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ycayttps.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rjfjcuds.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ljggblip.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ftemczky.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2rcohcjrn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ffwvknje.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wbxelkwp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2fjptnvvr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2xfvvcvco.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2hxyiowwo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2vdxaasqu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tcjoatam.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gxwncfrg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ijgqovsz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rfzxapjo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cyammmic.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2emggdvxj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2odxqwztx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2hqdwqmcv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nxydcjdq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2iistqkkw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2zhabsdgl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2acgzgxfn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2bqgcwobx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2knflxudj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2eznzwttu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2keqgvkfv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2cxpexlei.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2whseswhk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2sdtybdrh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2glqfyscv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2fmboipts.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2recqgnyh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2cdksrgra.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2nhfvqpot.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lwwzyysu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2cjkdujhp.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2fqrcegze.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bpokjwcs.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fwaxtmep.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wzkcnjyv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gdtuwwhz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2biccevux.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2izevzxth.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lfkffuqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwstjkuj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2uvvgeplb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzbnjbgw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ljbdockg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2pqmssroz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zsuggbmm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fbodrgtp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2glcgxzra.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2xujymjwd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fsmrlilu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2wytjikjf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iktubevq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2zeiixiud.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zlygydod.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2bvggizma.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hwmcxgqr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nabvqqmy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wndxbowf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2walsucyw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tliyuxsa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2fxqdcwrw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pjmsqkkw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2qeaoesqw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fcuywhir.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vwmikwdn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cseortcb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lnzfgovc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gmhbftiv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ppueksxo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xqhtvnao.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2desklxur.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zwogzsnz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2jinotchr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2bbbfxuie.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yfohaiqc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2oownvouo.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2mwzgdnhf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vuouoqgz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qlpdqwce.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2yjndyqol.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jnzsakcb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2piwzgfjs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ejrfmksx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zdnneqtm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wzqajliq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2fwwsxter.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2jpyhkxij.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xgodzmey.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2lxjbbkbl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kznrnhat.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2omvcfnej.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hcwijzmn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2osnbtjmy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ttkqedsf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nhwgbodt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wrtdgeoi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hjbpjyfq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2jcvdzrug.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2rbgjkoqt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zajywyct.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fcajjdfd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2tegthope.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2sfqlwkuk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pvkgzryk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2fhhtivmq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2mlszzjvo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ceomqszg.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2bgzgavff.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2hqsfknnb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bostlzeo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bcumkegz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pwwzmdnq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2yknwabhp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kmziqkju.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2yowjylmv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2klbzuajw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2jyqrqumx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2wmuhqykd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cwvoqwkj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rgyqbskn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mjloxdiq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2yowuohmb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pdcczpem.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2yuwgzeml.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2juhmgfag.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lxldqbbq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2jzcgppba.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qkqwooqy.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ceeukivw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hafqnrem.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tnljcaek.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nyduscyk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jvafusdi.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2tkdtgpww.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lygrskfk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jzzfnjlz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tlykgzcv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kmosdabh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qjwgoinn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dtxwjydg.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2sqntwyfe.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2egjnycuc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ahhxvqbp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2nfvxupmu.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2pzyvcsrc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hxffectv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hsxhgqdw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2wimnlnzx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xpnainpp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fhbfvpan.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2sfwfahbk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2owoentpx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2nzevfaga.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2feyhwyfa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pxipkbww.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdpjrroz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ogjghvzs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wiqhdxvs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2idkkswxb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jpibrtwy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2gotfrdbz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2wnkjcxtv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ronqwpsf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2vmgrbwpb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2utbetudz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mbqyroxx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2dicourrg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2etkdormf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bzrbdkyu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2hpccvrkm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2wdsoguyg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dyjrstmj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2mhpmrmvy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zguubjmx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2qhwmktvn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2nupuhftf.html


<!-- 参考信息 -->