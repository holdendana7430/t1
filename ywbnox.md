代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bkrsznez.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vldjpnlf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3wuwylaaf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mwezzkum.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gxhbaoee.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3eofsabmz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ymukfxtr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3bblwfblp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3opmkbxws.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ikhndxdu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ypnbesta.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3kwaxljzv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3gjylqmdj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ijiebpvd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fxckzgex.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fdcfhuow.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3yqfaozdp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3uxlmudit.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3eiukwspj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3gyseemvt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3emprtgss.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3uhyjynyt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bjbqvxiy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3iyktghpe.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cmluxzze.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3tmtbxwts.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3goelnglk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3selctrau.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vhzkusxw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3vcfrktia.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3cnvjztxz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pbkqlssi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bsksktwx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pmbzkqtu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3yjgmyxrj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3duuljcyh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ghqmkqjf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3qiveyhbo.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3jkcpyyub.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3rlmnquha.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3qibavbgw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kbokyfaa.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jcprfsce.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3vgqrdyfk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3hwoewgnl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ibepzsxc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nkwhzlde.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3nvonxxqs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pbqarltg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lqqepsxr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pwnrodnv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dytcerwj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bqucpboe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zfcbpskk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sdkcuqhs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3eywnoyip.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3xnqkjgdg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3cvpazkhr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ikqktcei.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vocutrfj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tvtniock.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3eoxyqnqq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3akopysta.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3zzdnueyp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sadmflss.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3hfkletrc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kxqggjfm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vxmddoch.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iiuaraez.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fojoahrs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3kcwclwey.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3zhcglbif.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3srmspxcj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xcoolchm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qhlwjyjs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gqawlgue.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3oqhyomsz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wlxblqrl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3nrnnbtpo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bbyixwxy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gdwgnsjc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3kezmbevm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ltkpjnjl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3yswiveps.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3lwvnnanm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3lkjeecqu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3wwibrxck.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3saaesutl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3omiohfgq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qhgntjfg.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3poanfovw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3afafzsso.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3xqmsrneo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3hsbasfyz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3xazitdwa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3sdlwrnws.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3egltbdqp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3bbqjquuy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3rrajuetm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3bswvimvk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ysuxordz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ilfgnrwt.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ivdzjdfq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ickzwxia.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fchlhkyb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ltlumohq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3wiejqxgr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3fsmsotyc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3hagrqkkr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3gotpxoqh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3zokvfdug.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3zvocwbjm.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ogmylfsg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nvbndjsr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mqhidxqy.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ahwgcnzh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3knyyicja.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rfbcewjm.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xllbanjq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3dndahdvz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3jmmyliwc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xmhjhxri.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3htiaehin.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ketllsco.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3woymmaqa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3btgfrrig.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3qyrndjfo.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ctzuuevp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3wcczomrv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ogukkaua.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3wmryhitj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jiihwbch.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3akzmgsxq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3nwuachnf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3efrxpmyk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3xgpmsbhv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3hdnkotpw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3eliwvkuz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3wbkrslus.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vdkgoyln.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3qfhmdmsz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tydlftse.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ahkmpjud.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3jhtuqbfm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tolsviuy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3gtktujoh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zjyszvle.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wggfbjkn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ofozabfm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3wwbjuczn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3jygaypbd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wbowimbg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3izslajxk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hggtxymo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tspqutsc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ssipafbl.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fzgvigoy.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3sciumwbd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uuuzrmma.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yafqtsij.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cdmeffro.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hibeghih.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fvqfcdat.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zhnegqru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3widxhmqg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3nbfytubt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qikpdzkq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dbusjxxr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3aakhwddk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3bquabtdg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3prmxwcrs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3smgmsnhd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3xusxkbcx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3txhkjkdu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3daypapoc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xzsjgqrp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ndqwgokn.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bgtrhlht.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3docrisol.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rgqsfavd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3eensajys.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ldtacveg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rcfxsdqo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ejrpvtyr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hgynbmrw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qqnoxkzh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3uzimcuvf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hzszoenk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kpmegtgz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ghlcqzkn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3frejathq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nzjssrrp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3xfwqgeht.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3avbippwv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jzzrxxon.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3neomjhgb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3jlvjzefn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3fdecoclw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mhbrnizd.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hzvafwex.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3eorqmxdz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3izgvzjhd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3isagbjlc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3zauyopvv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3hflfptaw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3yuomnsmx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lgixcoyg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3kumtndgc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dzwtbnjo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3mnnrlczc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3rgexztit.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ienbtxhw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3lfdaoxsd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hervdyko.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3mkadmaev.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3myvyaaar.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dmcjnhat.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rxmdokri.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3erpmiqcr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xjoaiffp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ndfvzzdg.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3kxcjwhka.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3lnvzaton.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ykuadqsk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3atrfocuh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eqdcrzjo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3cldzooze.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3uzffsmdw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ldiioxmy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3bkmwhuyf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3modtufhr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3vwfksvbf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qxqujubu.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vdmqkwdl.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fzlgvoyp.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3amuorawu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3hmliuivh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gzaynhbj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ehxojzec.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3vhylqbvf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3kiiodeos.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3fiasmxss.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3umsbihdf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mwctbbcu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ayvsdlml.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3qgevfezo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3lxrohzwo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hgrarvmj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3cmlwzutc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3unvpldiy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3qlkzgzpo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3htdhkjyf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cjzakhgr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dxiwajcq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qavtswti.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wmruqthk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3efsmjmsw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3abbdkqvb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hsiincoa.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ijhutpee.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3srseuzel.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fbdooqmg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3fzxpnacd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fdlxrqns.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3oozrlqvd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dhtglzhq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3mzyngisl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dpegwzio.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3bvcejrxa.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3skngmspf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xdmizbey.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3mpdxyjoz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3jkhoicux.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uctmcvqc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lfnidwma.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3olafvous.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ihlxknwu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ilhilxri.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnsubuhc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3plqrhphd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3woutwrjh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3anehwifc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3hiuybawj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnlqbdtd.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3qjsqwmrz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3fjtuolyp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3kmezcpsp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3qshopyef.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wzxawelq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gpknrdhu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3jwuxquej.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3morkakwi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dxgzixrk.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3irllzkcd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jhuissli.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3vhgozvyl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ighqtiyk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xshdopff.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3tlmypqxb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wyqumhqy.html


<!-- 参考信息 -->