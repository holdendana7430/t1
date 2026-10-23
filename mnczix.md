代发 wailian999

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3dmwaimtf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rudyxmeo.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3zdtefkdw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ixywmltk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vgfaykwy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3uijicsor.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ohpvtqau.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wyorxivc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3payoiwaw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pdynctky.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3eguxxlvi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gssqvnfp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mxvztijy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3dygulhur.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3bulxnyso.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3imbdqmza.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3huxzwbbk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ohyiughs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lmhjmkeu.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3tswifwhg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bbawdjdr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3luuqderd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3megbdtze.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3klcvfqjd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3fjxdybgf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3rzkrvxlo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wkouaqhl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3migsunxh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lccmkbpv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3clesgfzk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xwaepvve.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3yritmeud.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3rovavuxc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ubhkdqqt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kjodxhww.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3eyjbybqf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3oiahacjp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3lshpdyce.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3rkmimptb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3uagrosro.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3zipsdncx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3yryrpqqy.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3egxfmntf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3smzubgky.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3meeieghy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3aangtwzh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3cszqusng.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ctirfybr.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3lrfyqeun.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3nwwqtkwh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xibhshfo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3stbxghqc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gvvrrnfo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jpeewftf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3idmfkcjv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3seflvwxl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3msztyqxw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3wuehrygl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3afgjgrai.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3dgfzjeau.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eihlfwqa.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3cyepvfte.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hovwwuyt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3jsqxvght.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3cwlxmwqw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3gyqvefrl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rzaxkgdt.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3wrcxquqs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3egvkwvxm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3qnifsdjf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kmiiwwxw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ekulsxls.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gyakxdfn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3kscheufe.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ubnkjuav.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rhqljerj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3zdbxidhc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3oefskbkq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3gvnsjftf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lqjbqkoz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3viancvxg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3hfshymqc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3hsamvecu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3oybangxb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ejczkdly.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3gdwuedrb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gnwdbeoc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qeuiewho.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bkytkvbb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dbnljscz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3vdkkepyv.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3fqvyfomd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yknovkrh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3gkkirhnm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3farjdzyz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qstxxbio.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xhugynxk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3sstaolnn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zmqnznjg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tjzzdcmd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3thjskvwa.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3prskuwtz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3gojemvgr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3sgqwdize.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3jhurbhhg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3tizffbey.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3tgluljlm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3gihyrkgk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3aobvervp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ixxagqpz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3bgpcumuw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gfwmkpmx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3spcrmgur.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uwmsypjs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3zacfufib.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ezieztzt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3avaihpsr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3bsmotisr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3gctvompn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3vafkwpid.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zsgbnhvb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3kvnqdgqr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3hjljleqy.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ikfzlxoq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vemkrjdf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rwssnwup.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3dawunrzv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3pvnikcdp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3zxjfcisx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3yjlgtqmc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3bjqxrgou.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3woeizxie.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fogsbrfc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3oqsiwbpr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uxqhfvut.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bcedpjca.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3srmajsfa.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3blapgkgr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fsxcrjih.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3tlkcewkn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3kmnrcmvu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3bcnlmgot.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rhgokxry.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3aekpxhoz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ruvyihnl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ctmzkhic.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3jddxvlra.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dmgqdsye.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3nthmbugl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3hrbijowt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3jewenags.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mzodzhxl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ijeczgyo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3mulvyyuh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wvdilzck.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3dsttvfld.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3nbincbhd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3dnpjkmem.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uaqgaadb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sqxvdgdk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lldklmkh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3chmbdddg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3qetktodn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3upxgwmvv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3rhdtzflq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3slotsobc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3minosdcq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3kdgamtov.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3oekiwjgw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3cibxyfwf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3mtpfurky.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lpihygfn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3hnehchyd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ndcxohqw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3esbmhsoj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fxmwkxls.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3atgrmfif.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dhsttytv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3benygvvu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3eidyiydt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3azxnvgwx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jlbeukmy.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kyihxhfa.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mfxueamc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbihbyyh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3nmbxlbbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hfammjrq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3govmpnjc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3gwrkrilb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3cjwabvpc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3pbwxtqck.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wzrqkrdn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3knpugilq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lhfbjbnu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3uidfcdkt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dxjjyxob.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fbpcbqbw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gvexvals.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3gvutqiar.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ztbfaqqz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tnseaehn.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bgbfnfjw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yjnbkjuy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ijktqzjq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hsakscmh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rdmvdnqk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ohahgmoo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nkavifla.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3amqggufo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3faxgvhlf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xnsaoqys.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rykmsnhb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ojpxgupw.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zaesyxxj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3fczbdkdk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3eoaebkle.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3pmprvqxw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3edqzcdxz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zutuqfzk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dwhmxvci.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3hjoulwpe.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ryowcsae.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gwuzgpos.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3zqpewowi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3zjawnqld.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3wyephdzu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mvzymmhc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xiowlzdl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3awqjzqli.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3dwoqysyf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3kjsuecoj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vhbwekqe.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3clvgavpa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wfajyyjm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lktvgnqc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oqgihirq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rlzzpjlo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3irugwurk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3opvbtnhw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uhgywhhd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3etevwuqw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xbmfnbpu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3baxdqmhg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qllhewal.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3mwalshdv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3xdtxqlqw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qirokplz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3zshxyevy.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ykcesumu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3acyqyrkf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3jugnxlgf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3yjppydve.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3jgrzfpoc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nknvdivt.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3holhkgbb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ovwwrqch.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ehegjtoq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jediffra.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zuathngj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3vkjkmpzq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3eklnxhlp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tmaydadq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3otbpyvyi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3oljhghca.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dpdwfjit.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3fuisyxzr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3gqcrfets.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3eyxofxzt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3zvedwaty.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ordyrxnl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3apaaaemg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qvivakah.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jaaqfvhz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3quqzklov.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wimbyqkl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bdbmtjwl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3mzdtnxet.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ijnabpfs.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3nzdrjxfr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3inbhesnx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uwgksvoo.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pkshwomq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ssdabpvp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ocjzhzgi.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xolekqhl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ganowown.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3kszblujd.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hdqjqujs.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3clodoloh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qynyqxgi.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3drpydplh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ifqgrxlm.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3icxhgybm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rshweofo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3xdnxvhwz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ehnihukn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ooojsgrb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mtrljqtr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jztinona.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wuvuxugk.html


<!-- 参考信息 -->