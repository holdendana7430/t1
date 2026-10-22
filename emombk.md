代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2cygyacir.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2dnfdecox.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pzlntiup.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kaoxvjfg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zinnstmp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pjrlfshg.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2raeqayem.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2lksfgwvl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2bkipyzau.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2mnhwoxky.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zvjgrsdg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2retfkajr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2inzadkrm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2exmbdwkt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ufcfttfo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ydflxzqj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kqhefqia.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uukneqci.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2oqkowzbf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ovheplaj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hvgsvjzy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2axgneiej.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2gvstpujc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ummaispv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oaadrhkn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fovthtln.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2uynjcsbf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rcebxyii.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hitrlvgl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ygqrluyu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hcmylkdd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tapaxarj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2vfhekeve.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2whxwcnay.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2pnkltjnm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2mdauuzju.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2towdgmzd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2wkomhskw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2rxecpoeb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2zdqvtxkb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2gpkjxpov.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jlvzcwbf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xnpahfgv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2efozmpax.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2biigcuqo.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2mzvbesmf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2fxydgaai.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2euzdteti.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xnvgcnmk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gvfslkva.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2gypyviuq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lytzpira.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ehhygrnf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2qohrhecl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2xbmblcqw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2oezkwyhb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2boxjindl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vxagsiuc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wmaxaiyb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ndbqqtpk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2bztlmgum.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2kbquzwnb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sihnwcth.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2cvzfwzmj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2bfglppms.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2omfzuvyt.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2udduzdrp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hpuoakmk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2orqtiiug.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mtzvfpfk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lckuomle.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dmvbirmy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2stmhjavb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yjwhxwil.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cpuexneo.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jpctytfh.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2viomxkyf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hirfrrvm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2crsccphn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2latgfulg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kkfozzfx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2mvnqvjuy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2axfpmatj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2leuugpxq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wtwaaclk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mvitqque.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2kuokmptl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2avuemppj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vajvqqgt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ssvivgps.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2adaztduo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2oemnydvm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2omovdhny.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vsnxpybo.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2fberbavj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yzsxvouq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2opfcgnjd.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ikznlkqf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2lmgdmnwy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2icddaqgy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2rvscapck.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2xaandwcj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2epssnpcv.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2yjhtfatl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2sczthhcj.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2zuykkmjd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2nsudkyvd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nusqsoqg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2mowrydmp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hzoskvru.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2bceythje.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wwillhlk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ldkaqfap.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2soolisrp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2lrqyujio.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ofbomzda.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2byvuugys.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2zdayxggm.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ydqxrmhs.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nlgdwlbl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xyfwbkjk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ilzlsycy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2sxbfmoqo.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2atptdjep.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2xpadnxpu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2giuuvzmr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zebhgpfz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xxqcvqcr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2rprvqsbe.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cpeusemp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ppaoubqr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ufucziid.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cqejkzbd.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sstfcszg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qfseuzpf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2lnkkmhbx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2bqsgqbmz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2xhtcjqdx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ruoielhs.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2iydztaui.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2vfrxkmde.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2shmghkyc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2gbmxealx.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xmphhhub.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ylwfirdp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ancibxtr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cqslpsub.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2oseiacjb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ydsevoud.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2gdmdqbpv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mzkyqrhv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2eezbitvb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2baidbfiq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2uwuspbgw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kaxvcdze.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hzcjefpd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ywoliqzi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rswrcedn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2osgxmttb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ugoyalku.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vdeogzxb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ltrhuunc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2monowpbf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2bhhwdjqm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2uboxrrsd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tclvdkpd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zfoefaul.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qtzcbope.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2hbvunbic.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yuimmnor.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fjenahmu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fjfggwke.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ppnpqlhd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cuqshoyt.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hyyxksbm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2svlxncta.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fosabcau.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2chfsurwe.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rpzylirq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vnurzgpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkxciyvr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2vywamtrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bfjiuxwr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cyrrhekm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2schibvkw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2mofaqrdp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wxgttlib.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jduhynhr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2uvsdhcdl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2kusertdw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2uutkhzkh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kwgkgznk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lkmpcdbl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2kwvugdyj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2dvktoryv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gegsgrbv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dpvduasf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2izcmaecc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2trowwswx.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lxvvwezv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rkpigzlv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zwjnkskw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2tvctriqv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dshknhlp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jptygoew.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tjelapzn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pdftavox.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cvlqeptq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2yvtumnaf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2codxuqej.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2sljcqhgr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jwyesxhk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2wjhzrggq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ahjssoic.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dabmqzdr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fqjisyhp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2vlotxxmr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2beuorzpb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gasxqptr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2dtjeiwnh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2cofiskfe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2oxppueuj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2safobdln.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2iskaishl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2shgdbeyt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2irydqgmf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2tghacvbg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wbdxfuna.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2mlkegaeq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mdrbkfcr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2eoviowdr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fvtitpdl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yqqvxydu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oahtiuim.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pdccntyw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rpvdrpar.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wgoerhno.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tiilubhf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2nhgqmexc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fhybtgjt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lnysmktp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2hrijftnz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2iallpebq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2konkxxvd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2aloqntmh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2jgzfyvis.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2oyvinppt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2qmfenlya.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2yqatpcki.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vylpmskl.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fljctbxm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xcunmgkc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2brrvkdyv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kozgiiok.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ufmumqge.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2avavohqi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ebhptcdg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aeajoxmr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tddluklv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xfnjaqfj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jbonkcpy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2msnmxuuo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qidzvhcb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bmnxiwxi.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2yauajpvk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ovklrbui.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2oibrtlzg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cfhrpuyq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mdkeoncv.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2igrqbtyx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xzqchwsd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wlnmmvky.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2hvztxsjq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2mmflqoht.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2utloxgan.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2camjnoax.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2psiageyo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2thzphfwz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2esfjvdqh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mmhddnmk.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2bedpsheh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2anyjkdri.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mjsscgbs.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2nhbiysin.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rbggqcfc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2izwkrgzi.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wdllexxq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ncqugfwf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2qfhcattf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ftigzjcz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ggvfxydk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mxrzivqu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ezrpxmnr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2sodkflvw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwiurwsv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zjoshfxi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jsnjuurf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gadkuqeh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ncokkwsu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2umfajbzz.html


<!-- 参考信息 -->