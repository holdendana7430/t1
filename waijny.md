代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3xaqkqbjz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ogwzlxiz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3bjpodrrm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rvzaywdh.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ipljtiyl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ktrdwcdy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3tobwehbb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vakkblhi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3miqztvev.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3sndxzqll.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3pyewzoxm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3swoyiuyu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3jttcwxxq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ctglercz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jomkdqwm.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3sddunszf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3geltxxih.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3buvovktk.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3gpdsqbec.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mexzhrdl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3phcpepaw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3skrzvzvd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3gpcpzrsp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3jsyjygkq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xkjroayc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gdzdkcpv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3avojatjo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3vcpkqkxr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3oiavcesm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wiybhmka.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xbhnynir.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lgitswgb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qipqmlui.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3fedgqemh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3qfimxgay.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3rqcuxgit.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3lxqolstv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3mcgtfwah.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vjzymmcv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3njiiyksu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jzxxuofj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3istblnnb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tbzobmmd.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3bwshytfh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3pfurcuyp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3qlyxcjpz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ytmccprz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rtimwldb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qqvfuubx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3owbyjrcj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3krezgzan.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3unymkdbf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3eogcbjew.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3bremajal.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3tqdnbkhi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3gfjjforr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nrsniqke.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qpkiielg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yqrqoihw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3pffyaecg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3dfdbeops.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ftfwzixg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cqaonblv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3nemfnyqy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3oeckalot.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3duqkqbok.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3llegptfh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zakkftgy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3fwqakywt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ogjzuyyd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kxirknek.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3woitrkri.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3jgxhwtvj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ifubmwmj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3lbdtceyy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3uvgnyazp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cppgohjk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3devfeylz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3nyuttvms.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3eaeowzja.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qimoswke.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3jfslfzpk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zjuprryj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kpilqwdr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wstzzrpi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fhemedgj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3yfhmowpu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ploklita.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3bszgeozt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3hsloriit.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bzgvyiay.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tzevvqwt.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tgvuehjj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3nlpgdtkj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3oscmlpwe.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3zyqywbli.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mfbjnepf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ttoduaup.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3qjtoeslq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3nniiyxtt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3jwwrvoqg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3njxbotmx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3cujpslil.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3qosbpxcg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rpstjzib.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3agrasiiv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3cvukitsn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sluiybqm.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3smxbmpmx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hpmctiqz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3kgftagkh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3aomyicmu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3gnnpuzjl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3timayntl.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3uyjabpfz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3bqeezewn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3uyahcnew.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ovrpbawd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3takfthwe.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3kmisajia.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qahdrrbo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3muikofde.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3khgnpwbg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3nbxvyxtq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3fybwfzkr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3kmdpvxag.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3sydyduof.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vkxsfivl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xjyjcuyp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cuwhublo.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qollhezi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tfycwrkh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mckuaslg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ngltjglx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dmttqmux.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xutmhcyx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3keoukmmr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ysfeyqoq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xszkvvai.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3plpwqytu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3yedbacud.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3eapefbpk.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rtykpoys.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3uhqqykyo.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3otxqtunu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3vuxppyki.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uvnxmbsm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xtaocrbs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qplvyjzt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ktzfaemm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ugfsnxni.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3cvouzizz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3hsaefhvv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3pfxrmwqz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hzppslza.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tpcqrpkj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vqmqrdbz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zessfkmb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3nvkdpupa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3duymninr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gjyawqkl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ffqircfv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3jyxnlato.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3oyxekauo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zaqrxnpp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3voxnbkbn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3eaqzittq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hgtmhszg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3lucwuxjz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3fomojdqw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3amrinvym.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ceilmvzt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kpsyqixm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pflendmy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mtspifll.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ccdphzpl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qmpqezfl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ypzgeqjp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ntzbsdyc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rcxheyoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btxrdxym.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3tjmfdyzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gvvlfuhd.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bxmlzabo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3khlckgyu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3czptwyqv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qkbkhfyz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tgecxezj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3annyezzg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3syiqmnrl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3tqieppez.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ivkzzrca.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fraxdpti.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kzfxuqjk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3mngodxhx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aomfzafa.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gwyhlean.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3aetvdoos.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3movtccks.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zpxwkuyk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dahazynb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ujyifhnq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3kwtfzbpk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nsrofoox.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cqwacaxy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vqbszwce.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ocyzfnin.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zvncsjtq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3wsngkzzo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3lgwpyeje.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3kgahzlep.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mtzcqbvs.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3vxscmspl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3dgertulb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yviylagu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fsehuvga.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3isceazrf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pdbkciot.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ifocpezh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3annialox.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hixesbyj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3nnkzdozw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uhhgfnfh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3nonqgpuo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bmhggwuc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3izwscezv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3omemvuoq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dxumxrng.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ydomstdf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ziuvmpkz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3lguzgaik.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pvujlnfg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gwprelef.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3plgtppoc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3pyfzbzcs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ireyqpbx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hjritwmv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tumsawnn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3qdrjitmw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mrqczbps.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3wzsmtdpw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3khxurrna.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3kzosovbl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gddjxkea.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3zgwbcdkn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3hwmiiurf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3vpmhchyt.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ouiqvocy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3rliqznwx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rbhplegs.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ktosbegw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3augbwgep.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3uxcfdsmi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bxobnsiv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3twrhkxxr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3rsyzummn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ssvywmtq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3gdhyigzg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ggjsnwbu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vcwwhvhv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pkqspvci.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3dxaxcmgp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3pwolsswi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3umjhqasy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3fskepoyc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kfpvpqqa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3dujhjkva.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hdhodeof.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3saurkdis.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ysqwjxna.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gtagojxg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bspqlthu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ixpvxrbu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gitqsbsx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3iuddyurn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tfkqsqlo.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dhfsgumu.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gvjmdxrm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jynzyvye.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ikijkxlr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zbrgeves.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sfmvxbbw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3sjyzlsat.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zktxcbku.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jpeczpil.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zjqtytuk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ksjkvvll.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ymmrnene.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vwseepls.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3getkiggo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ofbkyedk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3nlqlsomd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3tmphsfcv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzgmawln.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3brxqppyc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gektoeuy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3taeiyubu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3qxzvpnxb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3uwdnukzu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uimeugkh.html


<!-- 参考信息 -->