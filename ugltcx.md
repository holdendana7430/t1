代发 wailian999

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3szkuyvtx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hyifkzrk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3kacisgve.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3eqsiymaz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3tkrhgpsu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3gnqzqfbn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3omgygzgl.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bqemwutz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bmzxtxsy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gwaluqww.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3xmsdwvom.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3nvbpzfwc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gzclxqyn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3xxyjropl.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3domgkfxb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3tcbpyqkm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3dicizezz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ttsjacxd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3gtqrmeut.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3dyykhfvd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lfpdqkrh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3blwecxbs.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3suhddrdu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3aisxcell.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iagyivuc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3illqovvs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3vkdifwsx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3fhaxjtfr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bwvijwlk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wabgjzsh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3yjuuuifh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3atcejudi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mgdyfwzw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nrswxscw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kcibqimh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3faijiwre.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ogqzztlq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3jfrboomw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3hubrgmjh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wwkyzyvx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3bmzwcmpo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ojeyhdyn.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3qcdgqvlx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3lvfbzzbg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ewlktlfc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3igbdimgz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3btpxojvr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ahhxijlu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xxazwbcb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3zjwngair.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3vmnukjpr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fafouvky.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ifcmyizb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gjhdghrv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3srdvgyne.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ddwbqrzk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wofzgrwm.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ivylvrig.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3htsxpfmt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zngmqquv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bzpgpjjp.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wyznzfvz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ixscnraa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wsfnwjng.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3wkfnwssb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3bbtzszus.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nhovqkqp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3hygmqgiy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3rqrtocyx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lgtsljns.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ckuzqeeg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3klikjiow.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3glxkgpxh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3uytvuykp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yjnoacwk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oqmvgixh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qfiyuwhm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jbfewzwu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3dcydmfwh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bjzzkjzb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mrscrxto.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3uaqkoxbf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3yadatwpg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3tsubspxy.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dmeuudot.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3mggxbtal.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mwdpbnsk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hdbhlizr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3clhpgxdf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3nlslwlfl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3cbrcvxxa.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3smbhvxbp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dijllqoe.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3qacyikxy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ktkhwwpl.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vcvjlfeq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dlcflzkf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xvpdfocg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dzbvtkae.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3doxxysuj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cufwjrqs.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3rpxhqyyd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yauqkjie.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3wpmvqjhl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nxtfwoxl.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3xkzwnvzw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ltnoyvtt.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3nqmzuuer.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ouziszyo.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lbejbpug.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ynglsztn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dfduuaej.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xbqkdsyj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3caonogvc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3yhkrbqma.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3jkadiqwu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3bjwfflip.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3dcmblmob.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3cbusabvn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3acecxjmi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fjjazwui.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3wasagsje.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zuchboqx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ykuuislf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cnmrvmtw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3nuuloztj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3giplejig.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3uusbrera.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3dvhqzkyo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3iftxswcs.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3cmdvcgcv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3emvzwsie.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3shzjshil.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uefzjfbh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sjaxiino.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kcatbihk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ztrlchqm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gciesojc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hpkdmqjn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3nlfuonpw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ffphukav.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ugvpcgtm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tmjpoezz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3eocdvbyt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rrkorepq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rnsdvlbn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ntlgzhly.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xhlaokns.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3idlkqfuj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3sopxnqvt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gsdufepv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zrrxeonr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pidysftf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3entkkfgq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3efldsqdc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3rawuxqel.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3japjkckw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3lkvubpur.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bimaovcr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lanzjdrf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3vemuasox.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qyocarjn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vstplhov.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3yrmsgmkf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3mocuemyc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3odyyuzmo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3vxwxkfks.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3xqqrityk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3mmtyazgt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wsgecmyq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3feonaqox.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3saitlcln.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3niwhaxah.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3cyyxmkho.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ilkeiumk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3vylclrlh.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3janpbntk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uqriwtfi.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cudlcceb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ginywurj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ofzhicuy.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yfxytpub.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qhtojrld.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mxoutsuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pyiirxsl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3abdjixqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nmbidvrt.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vxyypram.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3gtyvfwfl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3cbccwfne.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fcumsfrd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rpowarxb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3jocvjruw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rlbjdybl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3lnotxjit.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qvmteuhq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3dekvrzfd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lqoyrwoh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3amexpfov.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dasbsjja.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3emljtkln.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kodriwve.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cafgmpwy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3otxvmhor.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3zqlhipoy.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tttxxyje.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3hhlqqaxa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3iwjudnda.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3glwfrynx.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dingdbnp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vgaxbwyw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3itzqxuuj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3yhrvqpfd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cqtzeuqz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3lizhzzgq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3imdwsyun.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3zzmyfzff.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ojoadvmd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tfkqrhta.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xaswohzw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3tuxkjxgd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3smdorpkh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3niwxyqas.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3dbhqncmo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3yqjhpbvo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3cttwttkb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cltnhlby.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3gomvngts.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3regoskmt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3komvyhni.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3aapggnbs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jockhjku.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ezruoxdg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pcbocbxa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3muipcpyg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vsfrtukc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bynogcap.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ogqjdqkr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3huvwykye.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3imvkramz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tfvceosu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3bfvgnkjc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3gmizczro.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vsieedvh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hidgvipm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3zggvkqbc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3vzgkjzop.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3awjjdqak.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3xlzeffyc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3kplqgvms.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3maljcuaq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3frwhwfli.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3iqypsvjy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3orseszzd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yxgzuizv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hzjdpdjw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3hkihskok.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zolhalcu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3gzizfmzj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3lpzgzpdm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qdxighzi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3galpptsr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hupzvgqo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fqrvhagg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zmfrmbvs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ckjpants.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3vwjudwmr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nkqqrbqj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3psrvocpa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qxphzxtt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3agrwubto.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sxxlqymr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lafhpvtz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3okesqnpk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wrxmbyqw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3googxbxe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3qhbmkkob.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nzjolfpd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qwpfkslu.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mhsdyhlj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3duerwmki.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dhardjpz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qqtyyzin.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kjvlrzyn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3eyimreek.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3boyeuoik.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3onxekqad.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mwmqqzjm.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ieeffxaq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3uuxxkpiv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3anrmyvex.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3tnloaaee.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3zlxyifmq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3johsjnjj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3xfkdsufw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qydaujde.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3gauobejk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ulzgqnkz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sorxkngz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xeucbwtj.html


<!-- 参考信息 -->