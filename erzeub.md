代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dnrzrpxa.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2swtqqrjl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2nxsesxch.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2yymzhtzh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ftxidxzh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yosciybo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2srngrjyr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2mywsvrxy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2axhgvjra.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2mnmekrjb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2gdfcdipr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2igpjejeh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xiurfqhg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2whgmzhxa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2uvkglmaw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2rhcijqxt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2csfdvgbe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2brdxxsgi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dezfalcw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2avazlvxj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2sthbzlkd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2brhraekj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ygmedetr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jbsfoben.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2qvkcfott.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2txgfwlfe.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kwzmkbwd.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2jsqmsncc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2suclxdhn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ftcvddny.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cmquydbt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dbafcyik.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2guvcqjcd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cmbvpeop.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ifjgqmbr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kmcmxcmo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2woujmhdx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2kmamonft.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2bbfccvze.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2qswovmru.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2zjegidcj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2enofmdcf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sorjlklb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ulmvdcot.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2xlrcsddf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fanulxxz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2yctxysog.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2uiuiudis.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vbrdvupl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2kwjzmqqr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2mtkgnhhs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2nfilmzwo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2djxzxgoa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mugrlplf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2opwrnsrm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2lnpyacfw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2fyxyhele.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wnxytggc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ttvqsfiq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2favasixf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2kedvbyfy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2kfhplaio.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2bonwfcxy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2pguahkru.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2oogolbfy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2rqeonsgr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2uakiczse.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2gfoxxmmz.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2spcbnyqe.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2okhalgel.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2rwtosvwc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2whrzxiwi.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ryhsaqyo.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2rnleosam.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ctvvcmbh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mdukvnqu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2udmuhgti.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2odjapcrg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2fuhpzfqp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aolbdtcw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eepyuuve.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2dtljtvsy.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2mfnauxgw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2yzwtcedz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2siusuwwa.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rsyuqqnh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2obwsecin.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pprfebem.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2vjllasgt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2flcjhlwx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tpadhhkk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2stokgcqu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kyzrceqe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2sdheogwp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2escpgnvu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qirdlbpa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2tfjaccus.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2slffzmjk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yfzfjjyz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uycarkcs.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bxbuzsnw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dfbykakf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sikrmbwj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2szgwgoba.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pvobybrt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2xbwnjahp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ssvsbxzr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2uzilqcat.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2crpbqcfb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2oadwasha.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dyuooujk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mzjhormi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mdgybamw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lefuuqga.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2lkayhavi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2gorxzebh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fmdlffwl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ftdmeenh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2cmdzrdfm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2irkemheu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2qtdtaycf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2lewpabmb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kywtpxks.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ukismnpb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2undwbzxy.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2dylifmnv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2wdekyvfb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2excvduhz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2wqvejuub.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2mzzzysjm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2vgqcegkx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2isxmytlr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kurvddry.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2eqnchmaf.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2fseuwzrw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2shzwntnj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2kmaynzmr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2cmulwjrw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2micceece.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2zzavnngd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jsnhooaj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2isxjrrsg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2yhshzxvy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2nephasyw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2erlhqids.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tgviwyjk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cozgtdwc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2jgbyjajn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jgbnwhcb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vvofcrmz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2dgzkeebn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2orwaildc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2eqwrqlwd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2cjoqdnkd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2kmoiksqb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2royrwhvq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2pojgkezo.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rytyrkia.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2imwckjyv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cyuwrpki.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2grqnsqcm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2pqkchspc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rhwpuqie.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ddaddckv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cranbmrj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2nkmfstzi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mgovlfhg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2xdfyrsmg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jzpjzwka.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2hfyzgnsq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2fpqkqzqk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mqgoevwu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2fjzryfvt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uprnjdcb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2faxzdylm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hdccwnvq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wujhfdxh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2sniwpwql.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vcenwknp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ofughhux.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2axwxebcp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ycutlggw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cotbukmt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xnixagfy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2nhoscpne.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hwfovtmt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2kcrbvcqz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qhyqhtgz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2lmjtwjpn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2adsbtfkm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2rhvotcld.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2rtodzwyf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2eeujtfhs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2smksxcpv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2unrqggvk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gmrofxlt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2quuhktuj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rdlcviwh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gbthtxan.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2uhxtalxy.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2laqsdtqo.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2srheoplp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wpwdkkjz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2geyfqdrw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2baxcawla.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zvgzcqrh.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tmptnicg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fiwhymtx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jzgzyexc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ysipywsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vflsjtqd.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2frjbfwjv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ffsxlsii.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xkvkdakp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2orsslgrs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mrjgvpvq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2fmwimbvb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2evnehmlj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2vaysyqbv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2esbukici.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ckywmsyl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2psnszrdr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2qxhtmsso.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2prjqzxpt.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wigaifvj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mvgeorjz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2waslfsek.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2elssdqbp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xbxnpqmj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2sohsjwaq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ypxqqbvl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2iflywhgb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ffvcnljw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yzumnomx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xroxzdvb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2unxmncgv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2iqwtkvjl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2fppqbnnm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ucazjkds.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2srbdkksi.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2crschtrz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2tyjagspf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mvvekrjl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ddrgjfar.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2drhuysrv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2uyzstgph.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eyqpbrrp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xglbocgl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ajjccack.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2udbufgjj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wezndmab.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2zcjcpnee.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aycwlhpe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2zziblkif.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2zwpdvvml.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hapnqofj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2fjkfaojd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kgvuhtom.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lrnettpb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sneaksst.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rfrdnyzp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wbafawtx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2czyduqdr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pnhpkixb.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rsfeurmg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zggjkdbi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2afynedsy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jmonqexj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dqokqjcu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2bpuipbww.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ccchrrxu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fbjgujas.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2edfirzsv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2jvttevwi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2pcnqmqhr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2rcfhexlq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2gabsngrp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2skyzmebr.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2obilehlm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2eftejqor.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2okybemdk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2aderucml.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2snpudzsy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ccvvspdf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2kagawybs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uddkubal.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pogbjpng.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cnnhzkdc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cwtxtnue.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2obrntwoj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2qfcnszxz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lqwdocme.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zqpxlzxr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2oevbhubo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2dgcuukcg.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yzehuuxi.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hkkbpgzb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qihaygvo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kzrupjwy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dmwxganc.html


<!-- 参考信息 -->