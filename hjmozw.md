代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3wijfsfvz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3kaouqykr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3cflmsimk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3huwccceb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3fbaqclct.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dsxvwffb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3uubpjtic.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ghfnjymb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qucolsme.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ororgvxk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3fjylssoi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3tcnnxyxy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3idyspizm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wspkvbmd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ksfkehuy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3nxvuxnon.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3clnuzjzr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zluyobek.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3czoftvqe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3phxxegcr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3lpdorrde.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ehpujyga.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3zkchfcub.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3pouhyitd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3qtzdeshv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3vymcjjug.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kmmexzuh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3leopysrb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vwyurxcw.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3jhfcizod.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3povisbta.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3plqriymn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3lzfswrth.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3rscrtgng.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3igwhndod.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zlpevvuk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mpyziujo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dgpejiss.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3upnkpyxs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sogafgeg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3lospccre.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ghyidexv.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3lgoirwdt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jbvikehk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3dawgyqps.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bkhqupce.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3nrdvxfnl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gfyxykih.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3vpdhxvih.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3stapqibz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3slzprkxv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3fweviois.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3lcftianm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ivuxbxqv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ikgzfwhc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bjtxdrcj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3yvkufvnh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3vvaberaa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ohhepsky.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rorxfvrs.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3smmvxmjl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ndqrzlav.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3pmgtaagm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ycmwmdot.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3afaokfkd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3panyjnai.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3rrkixpmx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3gmecljyz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jbplcqzo.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3yngfcxvn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ahduvwah.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dkqsysfv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mrenpuvy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qwgsaoah.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3jhrzssjc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3nxtgyfhh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lcvccmvi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3jznuzfho.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3czhrxxhy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rbsnbgrv.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qxxpqpzv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3qnecxwhe.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3enrterhd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3hqviaicb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xbhdwqom.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3emufltwc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3fukppnre.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3cphbkwdm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3yevrreju.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3pahtaaqi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mqrpcvye.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3waemvnuo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3etuzkjes.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mqzvypdb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3sdanzggs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lbhgufru.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ujltnlup.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mcgpvype.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3gsqndsjm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3xmsaktyh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3reoypjmd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3vtjoxasm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3jnxbqxuw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3hfcevyhk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ktxjvmgg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ylrgiela.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3dicxbcoa.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3pomrbner.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ckcdxrpe.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wcszcjkc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3gdroswpy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vpneycas.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3odbgdtmz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3zhydhcma.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3jwcloyun.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vjhbjxun.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cirdwtyr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gjxwdmac.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qhuzjdte.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xrwvmpsf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vgpmgvef.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pmiciykb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pibxjext.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3mnpiqfrx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vkkrorbk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3tvanuaxe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ojwsqutw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3aqfgbzed.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3vufyjwli.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3dtepfnxr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3etaqhzyu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3zscrptzq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3lcpbnatu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rjogpqwg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sosbqtnn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ctbmwaga.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dmstoduc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3kxpiuhhm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3bajwqrnf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3unlzygrr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3xjsxtuhm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3sokdosmu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3quetnzbw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dazqmime.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3zyzpszru.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kebjnzxa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rzoafcbz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3zbfvgjgq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3clzfeisx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3vnldmuex.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3clahakht.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3somnypbs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3opxcdrjf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3xjuhwgrx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3iqnaqdik.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ulornrzy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3nwzjjfkh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3gqendawz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cixbpvke.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3xgeqeswy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ygflwtwp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3keywaarm.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3suhnufzv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qiwuobwv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cirwljxx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qevyasvk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3btxvtmeu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3swnszpik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwjyemby.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3itrsvewd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yytgzayq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ewjafucs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3peqricmc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3aqejystu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ocjbekjz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ezmrqfyz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3knlddlcs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3tygelcrw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3mqdryrbz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3glhejsbf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vcwdxjzf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pcsqszsg.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3wlsjtjod.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bjdwxwfl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kjnxsvbx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tbvcatze.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vykonjgo.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pxgndxii.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3lrtiomuy.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bezsdrmt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3tdevsggl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kistckyg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3neilwlkd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gntwufry.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rxsryfts.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hjkpzyuq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3wwlcbruz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3hgrjlsjm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3rvjromqf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hxotakef.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3rziwszdo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xckbuzvn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dewsfbjg.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lxlqdkea.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3phiytiuh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tjivzdsy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zxujpoym.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ubtnypzu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nrzbvmak.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3mjfmdozb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lklbkbjz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lryhwmtw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iudsgymt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3invimldh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3vuxibagu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gjtncodb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3blyulfhr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nsrqlisr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vxjukivs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gtyxvosr.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eebrbxck.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jjdnlphl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rbihppvm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pesywelw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aegfzobv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gxpbjxjz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3razbaxaa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xhnxafeg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3laxcwwdq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3enhzjhvl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3lufmbjcc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3twpgrdza.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3andjfseq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3jterjemz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3jufldtir.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3zfmyfxfy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3cyzcxitd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pmqudnah.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ilcflefm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hnazprrx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ggouyauc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hvckysxw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vrprachp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ustknjva.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mquhqbfy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3nxdonkfe.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3phlrjvov.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cgtxzvaf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vrzygxft.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3iuomzolq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3syksanij.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ifaaquht.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3wbgyhwbt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oexflovz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3yehnkzvh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wfuxlmoj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mfbujxix.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3uvdeolji.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jbwdcpcq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bghwkroz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3wfbgdryz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3rpglkaiy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gypdxpxp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nlafibau.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mivwzxgl.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bkuyxpsz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jveaxqfr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rgajnyoq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lcllzdko.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3unujmlhw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3veaafodt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bmrnszoe.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lfqcnjww.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fthczoot.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mkuivdua.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3zmdomfxz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3dmmppkeb.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3yqqfsyez.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3tnmefulx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hwfwfvbm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3hmbtfzlx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmtreijz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mejnrsrf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3reshxgsp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbgbxdso.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3scnqmdjh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3odxrwadr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uxqhngjm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3pvjmzfkb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3nhmoxcoy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bcbgntnj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jrrebgjb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cjjtxrsv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ebqhjxlo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3wcsukbul.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3olcaopwb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3duqsggha.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xbvzbyqa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vixbwziq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qrbtiqin.html


<!-- 参考信息 -->