代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3wlwbtxbw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3gkfakljf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3evveclcb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ixeasnfz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bhwrihms.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3okafxgwb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3mopysdzk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3yvnijdeh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ovodsodr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3aelzhifo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nobcxvdi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3sckplsjl.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xyqjppcp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zuwbugdy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dwbvmkbo.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zgcqhzuk.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3hnptynch.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tmouadff.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wynusuii.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3uleaoxgz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3nhhczhta.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3wgnsndvi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fonyfdog.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qbvlxpbp.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ramevzdc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3faetdlci.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3kxjrkrmc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3sbcxrgkv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hfavjsyz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ahirdrfe.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3iurchzxl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ciupqine.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3tfvwxbmp.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3jdogjrjc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hohjwsph.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3danjzpbr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3hiagsbyp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xznaxlkp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ytuyvkxo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jyvhloud.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3wyvxdfth.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3cbxtfghm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3zstjkzqd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3shoviwpw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pedyvyzq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3eullnyvi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3lewfmhzt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3egkldyoc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3axgeyuoi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gwvjzslv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3txltivht.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ngyfwrqo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3efuovwih.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3yztcvoha.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3lzalbhqo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3eegmefew.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3rzctfwek.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3qqjnfuzu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jmuqugfb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3mycnjwmc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3uucsbfsh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ttnpfuly.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3lvsoomyi.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3zawjkvev.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3rgvmtolw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3dutnolda.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xvtoijsi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dvwfyzmq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3otqhgopu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bwhshzbk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3lnirubhz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hcngwiwl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3pqrppjys.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3iipmelbg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3usqkeqti.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3jhicvjvc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3uzqoegiq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ibtbpiim.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gtolzdxw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3twbqmowt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3tzfjhmwd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3vyttklqe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lzsthdes.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3jdvigfjv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3gpoghacm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xlkqjtlr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lrmnwqtj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rmdrugzz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jakkavlx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ceslavxx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3klbopvjy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3chreutzy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3znqjidig.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3esyijjib.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3mjcswvhm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3niewuvxw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yqzgxtjm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3luupqjmf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3lwglpdxk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3yjyyyzju.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3tfqaslvr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3lvstqysa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wwagbrxs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kfxlpqbf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hqqltkfw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mszvomyk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3phpdcfwu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3hqhqalwe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fgumglyt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3yxnvxzqn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3dobdyqnp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hxornpnk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xvjmyicm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cefsvbrx.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yjwhqqfm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ybkqhzpr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3urwcastn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ealezyzw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3imqbtflx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ihnypyfy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3nzvvmzjv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ujexcmuv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3twczbzjr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3xnjrqigl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3riepujtq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3hnpyxtgr.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xajsejlb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wzcoilgn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3cqmjpvqw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3hynxrntx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ssmrzbev.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3wsqawtta.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3mitghrdc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wthljbpb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3eorlguyz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3cmjazrhr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3szoscpro.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3adpalivi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3covixmpn.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aqqzptrg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bmyywpxp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3unobkeji.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ntcadptg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3erybcmga.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3tkvstjdc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3qwcbwukh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3kbrsyhmk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3leebfduc.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cofrkuiv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3effrrimx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wuadjikk.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wribobqk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tmxgxcfl.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3urowqljf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aezghjau.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3gjunrppl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ruezlbdz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3vepqtqln.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3hjzruoky.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3xzaiwmcy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rhwsrndu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3trunmnsf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rrtzzztu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ensquhyt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3wcmfugmg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mwmpotge.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ovabqhsc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pfnvodyp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pjkqsmwo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3jfzeoaij.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jxljrzic.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3jwmhfwyu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ckrkxntp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3wjkqziki.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3edhyjjch.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jjmpofgv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3zbcwfvhl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kcpitded.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ftabguik.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ndvhbpbr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3cqlbychv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3kyvazrgu.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3pmhgyavh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3aunhwayc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3sgcshwfv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3pajmvbpf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ccvpuqim.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3gwzfpnaw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ylgdpgta.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3asvkzjfx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uufqfbhu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xusxszju.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ixekbada.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qxxgvezm.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nukvyvmd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mdsmsykb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qjixuzar.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3uobquwgg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ydripztf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wndfbanj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izafbkfd.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3phsexvmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qghwdjto.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cdttbuad.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ptaquaxn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3tlhspqlc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3npruepvp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pmkhbgks.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3qpdmeoys.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3stsghpac.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3lkksciqz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ueposudw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3gwyqpgmi.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ierydyvb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3apoaxrdy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zmomwicc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3sjbagjja.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pihhaqet.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3emsyarbo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kgityrqr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3kbumoqas.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zzkyrcho.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3wchpywsa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fjmshyvs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mbfgmonb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3taxsirkp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xyssizms.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3irwmpwki.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3wjblhtuv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3nafeylme.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3hajbummq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fnvfifhh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3oygowxek.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ihshlpwq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yugcubfe.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ypqwyapu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3vigqngct.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3muyyuapb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zihkldnh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3krulffew.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vtuxlebq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3umuowacm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3emtdwxiq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qsuqwtvb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ntozjsyw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3tinvyqdm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fzkbjiko.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ytyslbxc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ivlclkpa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3eteffrbt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3fdjvxnra.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rogdprlw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vfdpuond.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qtwebxgb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3khaijbcj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mfhcoqmq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kbcidezk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3muizdizi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3lynypmfh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tzzpbcgl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3rcjsdvgp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3oojftwlw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3nekkpiht.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3fqzpfcgk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3hpwyrrap.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3wzukhdyx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3qzaautlb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ermctbkm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3rsybzzfq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tipkdgbn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fmkosryd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3codixagr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3mklnqist.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tsyahgyu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tukynlyc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3gujeqlur.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vnjdizka.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3yblqymnb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fmycvhhi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qvyuhmyv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3grdtwijo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3qzzajuyq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bzkzmzfu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gzoxjszw.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3qdiyvslw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yptwoqeo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3wuulzduv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pxsxvqmd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3isyrbxih.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sdwkgrlb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3umihyhuc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xkhcbdee.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3jgskuwkl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3wvrgamrf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3unhyroeu.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3akbhdpcz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kwerxwzu.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kifffkin.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jwcbdytz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3eulfapcm.html


<!-- 参考信息 -->