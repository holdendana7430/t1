代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3gwoxckte.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pugwrwjj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3nsvbbtmz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3mkjccszd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3cqacqvfn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3oxuvvxks.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3dlalefvn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kyxrfcxp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gxmupefp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nslojkeh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ruirasnr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3jmfygizj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dnrypxry.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gnbxxbhh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3resoqeoa.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pjqzxgah.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3icsdgvxl.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3uwrdufjx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fecbdtqn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ieyvzrtc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3pfeobpfn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3grxiuqrl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qeinisye.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ybttxwxj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ikwgqrja.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3lrxjnucp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3chrizzcf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bqfeddrl.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lzvplyvx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jygzskbj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3cnujtyus.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3weuzphni.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qxjgifiy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3xeohwqtw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ctjgrdbo.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3svccgbbm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3inoufukj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3lhiuttmx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3wdvbxdwa.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3vtvwbsua.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3szomjuez.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nwrfccji.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3bceqbnje.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jwahzpmf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3yhbhyjga.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3oufiirep.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3mbngdtag.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3rcipzgaq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zxucdugx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rhuaxczc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3bgockead.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3yrxsiskl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xeykiiui.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yjfslukf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wlnxacpo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gtfdallj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3awwberld.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rzktugdk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3gsdolwyu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ssatizyo.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3tlozshfa.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3rrkfodze.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gaqwfsgb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3rotrksbq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3caosjebi.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3svitxboe.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3gehlcfdn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nxqhnksl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3lwvgepkj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3gxhmrpll.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3deuctpnw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3niefnicv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rvidsasu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hjedonwn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3agxkllhl.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pigflzjc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ucgibhhe.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3lvowenrw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3lcifylrx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3txjxsvpe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ferpzicp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tqmppelm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zqwmngcc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3poobkyux.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3yaclqgwl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3boqiusmw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rwlvkyav.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3vrjzfmzb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3cegdbwxm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3uickbqya.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hnmvyfop.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ewxiwamk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3udyhlxnp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lpsvoxvz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lmvrpuho.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jwkamsym.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ybaqrkvm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3pbhwyozc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3pjppnnht.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zimhmyoq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nirxyzdp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ozdpcnwc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ygjnjyjh.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3dpzxiazp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nxosqopm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3fbjrprap.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fcaubvqz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gbrohzzf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zqspycrd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xuvcvlux.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3xukpxxzh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3vlznqtfu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3oizfxjcb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3kjflyuzj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3dxayycda.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wlksqtgz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jmdlzvrt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3lmdjccwf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gjzwmswn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3smoqshyx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gzyjbtlj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3niojwrpa.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3iiijdmwe.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3pfokwgaw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3hexycpil.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3qipoezqg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3qpzivkoz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3duglqfbn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rjseuqmi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zylxukmk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3bogxpaga.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wkxsmyuo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3gwkxlqgf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3avalnher.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3abohvvtl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3qhhgrcoo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3cmdbtttc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3orvqhpru.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3declores.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ickjmavn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3gzkwcauq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3blcussgw.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3aycrsbtt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3yretghwt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vnvktywf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3klhvxshh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ppewhjme.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3wnpmeltc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3lpdrhbrl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3vlzlbphv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3yhwrrjef.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3axpfonmg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3illthmow.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vzqxglqy.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wvrabccq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yifqqbwx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3usrvknyl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3oapdmnji.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bocifizy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3mqtzizdf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iqlixrkc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3nqnoelqr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3dninjalw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3niwrfldq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3bpftnmzz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3lxhamnkk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xslwctjd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3uqjtlwyg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3bljeacnm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3cbuoxniw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nimrugez.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3yvglbcco.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rjcsldps.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ityhnene.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3eprvrevj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3gcknujkv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jumijgfm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3flpqayhi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3norhruod.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zcrphfxz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ymnminry.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gjdxxvzq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zwddofll.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3wyzapcfd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fqxxgmdu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3xxwtnkmg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3mdktzodm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3qtxjggiz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3htotviut.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ydkbtwlk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3earpuvop.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rqpxxhay.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3dfmhhmlh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3flbchlmx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vjskefak.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gporvdjt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sydjfkwf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fprddzyl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uvojbbdr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xxqdartl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tgpoifyj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xszopnoa.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3owmitkjf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wpzpciou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elnqsjyf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3kayikqwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xthetkja.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qrncprnf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3kwtjygzl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ioxbrier.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mdtfsvlg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3icgktcez.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3lfcksbxk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3moemgtty.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3mezoeeql.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hyykpdrb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3feocbcxe.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vanaykzg.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vgcvtrzg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lhjwrgoz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3iispjglp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fwefrqyt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3przwstiu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ympzsaee.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jjveiuhg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xlxvlgwy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3qwrghjlb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tzzdsodp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pdzevqic.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3farkqalk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ebcxqzql.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fbpefsyv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3fbbxijzx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3udobqwox.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3gckljoml.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jyqemaaf.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ymxilajr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ugjnrcch.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3riababrw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jffxedvc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3iohbgcjq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3snldhzfm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ijjuhgiy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3pdthngtq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3gaimhmko.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3yjpzhlgz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ktebzyzq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nypjgekz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kfsgzbvh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3mufhxmhp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3dpavoxbz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wiphpcgy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3adzmzzvt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3grtkqpvk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3alrgtnxg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ggmkuoxh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3swbcwrni.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yscvuvqd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dkkfjpcs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mqpqufya.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fthzjomv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vuvwdkxk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3jerbuksu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fonazzqk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vsfgoeew.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3hctvlsav.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3jiivgvjb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3pcclxudv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3zilvipyq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ebviihmc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3wxvvtvox.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3wpkdeaaz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3tqrjklne.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nqcfpdhc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zqnzdtwv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hwfrakuv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3hzazfssh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qexchixc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3gkfcwrjl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3aipdusxe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3svwxofmh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3crtgyxch.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3alpwzelb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yasyjiet.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rvwvxgkd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3qznjzzsa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kcuwlagp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ktehesaa.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3icassfcd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cfdgtvgh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3nbdahglm.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rdekyfcr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3reytlzez.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qniajeln.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pwoxszoi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3awmyqedm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ateeayqm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bgamztyx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pihseofv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ancosajw.html


<!-- 参考信息 -->