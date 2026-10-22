代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xekckihc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2inenhzcj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ragluecc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2otdkzxyc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vtdcqgnf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hawydrmz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jscvzmhx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zlqdqamp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eblrykyk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gqqdiihm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zikiyxmb.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2liqucspv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2vwdcvaub.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mqobhkfh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2surqxcjd.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2isifofdj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ekzbxark.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ktmqlzww.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2irhazvsz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kzuyizes.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2phcymgeo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vpxnkejx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2lpohxhmw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fzirccxf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vslxnlgn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2trhytide.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2fnidieiu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2dnszykdc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2vluxjmyc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2zqfddnew.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2jvtopmmg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2txzttcap.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2axazlhsq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tgahlfbo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2crpksixz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2otyowgdt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2opbwzfgg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2dsmbjaky.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2butfqkvw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2udkzlbdx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2waagdbte.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2tzholsjp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2nsonawkd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2uskghcta.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kmzcdfde.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gdrtwcxt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2geqkaccx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ifxepoyo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2rgwjlucb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2kiauifbf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vvmethpx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2enaqpqjk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2hqzuxgxa.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2wpodwuwh.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2doeaxfap.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ippkdzxm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2zbtcfofq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2saweoang.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ikoyuxts.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2habllpin.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2lfbfjzsa.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ktseshbx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2sgyatguv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wflrukfq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2plhhdgup.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2agvbjeze.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2slygbahs.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzzwogdg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2mntxfjty.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2vhtsfpob.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2hgqfygzx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hcumhodc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2utpndpkx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2omoqfosz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ewjtlrny.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yqbjfcpf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2kzfqggqp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2kjljemjq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pkumqayz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2rccpqxrd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gxumtbkg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oqvdygae.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qzpyrjpv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fqazuzui.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kuoelauf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lszmpomv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qxwcldja.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hhzrddyn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fsovfjtk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dbygtfwx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vgidcmbe.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2uzglptgz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uxvuvsnk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2nncvqtcl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2vbqagfrm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2eknmqddp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xrqecvla.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2lztgaduo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yfpejsld.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lmztnory.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dtprvayf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lfhaamop.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2vtuitzaw.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2oxuejxvz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xeaohpvl.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2aqwloecn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ywygzklm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hygsrmzz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2qfaxzudx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2bvnolpan.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bmmxrduz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ppqlrqfc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2okhwmxrk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2kfonjjjf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2hayxvmvw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2hjihtdbn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2xrrmeymj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2pudbtimx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2quyytblm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2qlikggir.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mpfbjmmx.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wycumlxk.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ieccxznu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ohnrhdez.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2fkeoozep.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hyuvigbl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2opfblznu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2fjkmvxun.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hdpvujmq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2eogjwjuz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2cxwfipnt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2xutcthnt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2qfipzggh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pjxormaw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hngikjpx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2teytgvgq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2eajbfkbv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2eowlxclm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2nalcgaft.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2dgqptjzg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tstyfuwt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2gloedfwn.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2euozbpjf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2tuodhdqy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2mvwzhkea.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rbzuczno.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dgcwafkl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tvgekkos.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rvlunbpx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zmdftmkl.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tvrbtdvc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2plrmqshw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xklmhxrb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ashdlbhz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2nqjhfivh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2wjzbhbgd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iticnrxx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2jubyhqob.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2vavaygmo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kzafnwax.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rvemlber.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kqmivrmc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ocqyehsn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mkkxznwd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lxwebots.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2amtgqjbi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vabpsuas.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2xgnnmkhy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2nomzzcru.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2danqwwga.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2pafbslgc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2btpauqbf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2mefpphue.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2urgifise.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bnjirmbm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2schtfxuu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2awenecby.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2xrauhfle.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2vegneokx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2tcowuozp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2gpsvtizh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tjupgmhb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2igzmsfmf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xnlwtjmg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ntcjojeh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2omyrkdiu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2luqurzpj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vsvkpstj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ajljvpvt.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2kitckobx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wmptpccn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rfnzjsbu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2kdialzmh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mquukmrb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2guarfmqz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rxtmxcsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smrruizd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2rwsgsthu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azgtmgao.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fvmmrwdi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wtuisbgm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2bcpiaehw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2imzkwbpz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rxngyhwh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2whwsgmki.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2tagtfmtu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2uafgasfp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uiccuhzk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2evapeqjm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2kpilmwiv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sbctmrrz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qmruenxe.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kkcxykqv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lhaqlfim.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vzxzxwvw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2figvldmh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2sbtrtock.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hvfvqtae.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2cepeorlx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sytzhsls.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gfdannvj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ztsgjros.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2csilfcxh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kaykzldn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2wigdiyxf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dxhzhzes.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2blrvfhbd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zhvuesmz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2vmhctkeb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2uabutxsg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pzgqiljj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jjdgqekq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dxprybcj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2avfoxoez.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2paumbegz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2uotckazr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2awjbhahy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2qjuhcqtc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rnyfpbkv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tewsehpd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2oqqwfqvs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2gnrlhrvn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2kakplntw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bxabyjsw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2vgaqhkpr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2oiczqibx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2fuxoreok.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fcgbnhdm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gcyuzqcl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ixwqnasp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xbegraai.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zxkqfpwl.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2grlpqple.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2wkyzabgm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2kiflkohs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dwzhmvzf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ebernkcl.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pibyqyhk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2gymjflyd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2nbmbwvxt.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2kisibcbo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ehxofxmo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2vchinjdy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2nhsgdukq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2qwxnfgox.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dhqvgabq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cpargrxh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rkqzfhsb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2lbupwvbe.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ivyscayx.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uojkcsmg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2khvpwuwy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jcbpqwgx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mcebptcc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gwdyfgzm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fydysfjw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2grybvgko.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2onnqlets.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xovfsitl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qwpxaonc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2rgshhzjh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2abwanomu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ohitavhc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ktuqxuhu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tzpyetjk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sslxktnx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ikxloaif.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mldehxgf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ggwussbt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aqraqnew.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ajbicihf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rsihwnfk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vnzmjtmy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wuczjqrn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hikuidli.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2oqegyyda.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ohwqjasi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ukqazxts.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tpizliqz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qzratrzx.html


<!-- 参考信息 -->