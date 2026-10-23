代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ubijzuav.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rrspdcql.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3etoqzdtu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3nehljiwd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ksnddadq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3vjpdhvue.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zlizudfq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3geoasnlv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fcurxthi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3sagxmvpy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3xxuyfibm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ohfzxhej.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ikohgwzy.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ypbmkvjw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3trhfnpsu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3zuddprfu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ryvbhnth.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ymxclkdt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ktatocnf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3brfkaliq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zowzqves.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ewpqoaua.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3vybpgeek.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rvgdhnsr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vlotzwuq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ontpmmwx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ebbayaft.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3pzpzesau.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3aafeidcv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3acfcbobi.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3gjhyeywq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3csrdvvoz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jofvyuhd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3roahbdty.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ordpqyyw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3zyhjbeut.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fzppkxpm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ecjfuuoj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fvpvswox.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3seqswvmp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xmrvfnnv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wvwoywpn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xwhhsizy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3lkgvqdsa.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3djnhyrja.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3imtjwtun.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3mjkvuoou.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3rsdjtewj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3jmmcuqgy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3dfavuzee.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3otdjghkz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ykjkzizv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3inzaxriq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nxvxnrie.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3zjmrrwfe.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3kibilpxw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3covufegf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3dpfwwezk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ecslcfbx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3aojziomt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3jskaoagg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3gthwrars.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bocwhfkn.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ntpikwsc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3bylhwvwh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3znhnppkt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3hsftiobp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jaddckfc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3nyystwqd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3tfbfjpzi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3qbitbumc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3hgpfdjio.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3erinaqei.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qbnqbsxe.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3tmpzabwg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jwmjsfrl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3mtahzjeg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bbmyxlnz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gqishsil.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kstfotzx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3plwlwvbm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3jhythhxa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3hkdwwuzh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ipnapaye.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3hrdkcrmo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3svhcnxwd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3kcfaqsbl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3jmsexgws.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3kjzylwgv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uodeejqt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3bvhlapum.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ofgphpqy.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hbxfouzp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ebducopk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mdtbebpx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kqhfmvka.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3idgejekw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mywkggoc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3uhtsfqgp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fkesjmdr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lrhnneyk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3rluxodku.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3stsjzkrx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dgcsvtzk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3vnurdptx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wtxcfekf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qmnxafgj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3hygmnidk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3zfimpgls.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3vdawmegc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vvndauuk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3udyvtpxl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nxafegyk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3czsfjbqn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jqsjmxfd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3srxosuca.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3knvurjtj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3gghdyjpl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bzxfcbaz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3atkqvsmi.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ebyiejuk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3luvvwglf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3qelmmjdm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lruvxjqy.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qztbbukw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3rghjsrjm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ixfgsfdy.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3trcdwfro.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nwjfaels.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3wqxjkptd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lhizgcqy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ruihfnum.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3cluwozfs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dlnbnjcq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3fzbleirh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3lnzbauwg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3amcounlm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3bbcmiqgm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3sewbcnas.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fksggoml.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3mcruqsvp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uayebexu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3tpwgkcvs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wokluedf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3khdgealt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kiovfabj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3iyxawtbf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3liarswtw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ewgwjcxw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3pkipkvgo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3sagfplft.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3jmrxwrfp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zioyitjr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3afrnrsfj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3bbqfwnxt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3befuzrvz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3bolcflmj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3njkpnzla.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3mnrrpsaq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3rwzfctuo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jtdogtec.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3driskyla.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hxrxziyh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ttrwhrch.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3udrlcmnu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3lngpfetd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jjfmnxua.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3yhygffqw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3owzsqilk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jcbnjibu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3olxfxtjx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3fovjwgun.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3aszidhkd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3knnjskni.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ldetqyce.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3rfshkfen.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jlxrvelg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cwqzojmv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mwrryxdl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uxuefrnz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wskbdsvj.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nsbhlivu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3spxnjbac.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3fghqnqzp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oyibgint.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ctqeylyl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3btxaekow.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ambzddfj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3oaebekbu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3gcwmtgeh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3qufphvvq.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ukgpgkzw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3iwmuyycb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3jqoanxlf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xtvhftdt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ndbofecc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fyrhlzju.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3fewqmhuv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3smcvuicq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3jihfuxms.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwedyrio.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3qyvdybce.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xjwltfjc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mxnnwfjw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3dsplehdd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ubuprskw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3eiqqaauk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3klhztizz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3iugvwrep.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3qzzdkngc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3svjumrws.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3odualttc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3iiwitsoz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hkeqvbdj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3uhoyvmjd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3azkkojsm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3chzrnjfz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3jkzzzkgo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3uwtkwajn.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3brrarqtx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sipuznnl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nghfsrha.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kphbcsep.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3eacxzuhp.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gwfifprp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3unqilxxb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vkoepmps.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nkrfxeau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krfiyfaa.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3xhsgdwox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rimcrznn.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zgpzyuui.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3vrslrymy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3zxjgzgya.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3niudxxjf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qsefogac.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3unoijrkt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3oeufjkoo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3tbqftfhd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3autwhejs.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3mjvhymif.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3brismvfv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3svcfkbai.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kicmtvja.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fiartsgo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3otvkutac.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hmdwqfpr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wsgqrhpd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3bnhbkzon.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ergvvslo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3hgmkmdug.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3eeaukwiv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3plyhuiel.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qtgruodv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fdfgrdcv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3queccgnx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3rvrlmwqw.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3inkgcmcv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3xslvetlx.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3dzgsvspt.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3dhggszwc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3oruelszl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mxzbjjft.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3aiodcdyn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3cmkaixnv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ywfmdmsq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gshacbje.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3hiygcudv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3saenuiiq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3xmpqfczc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vvcgpidz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3thkisuwt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pzwoflzh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3mmqvjhhb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3symowmyp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ppguvlri.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3zzqwowsl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3mdwdinev.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3raqndwmh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wacxnxtx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vyxecrin.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3elllhpqh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ggcxzvtg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kjmvrcac.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lfmcsvjd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3futnsysg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3cldvfyvn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wrtjqktx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3nnnaitrz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ttkleuas.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dkkcdeuc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nuiirgtw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3venkmajp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3yibnbpos.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ettpiojs.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3tuoyilqh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qysykviv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ewxzbmzb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zerqvjij.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3mdxnbdbg.html


<!-- 参考信息 -->