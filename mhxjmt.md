代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vcelugig.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3veqrrung.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3qvnxghhr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3geucjpjg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ihmvrnaz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ashdstxr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3zvwdrhkl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3rvsofhtx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3yqeveitv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3skfhekmm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3svdjwjad.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wpdziszh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ogymkjsw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uaolaasf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3kxpehsqr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3kbvrnvye.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ibcbufwu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kgnpokuu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3hcvmoutt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ioyfnxwv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gsykmxck.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3igozpoji.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3rhwnmsvf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3pdgcleot.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uyvqzban.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3vaghpbsx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ertufkix.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oddieewk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3qctccilp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3qkmbukdn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3lvevcuqq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3skvbdpof.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ffatdjip.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3xwesniqj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3singjlll.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lxkrrzij.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gbtzjnsy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gnpsyjem.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3bzqldbmt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3gleuaony.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uesevofd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pnqrnruc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vrlxvctr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3icouckop.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ckafyoqq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3oyczlqco.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yzuscvgf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jyomnvaw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3enrtjctn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jrphhbck.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3eejvghkb.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3kkexlbqo.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3lntrqrdk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3mgkoovai.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iciztfnx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uqmdzpdt.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ewhxyqjt.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3huboiaby.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3cwprwaok.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jhjaucvh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lzzqqlzd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3cbwaktoi.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bokzjbtu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3iloglblc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3swvheciz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3fdfqlefx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ofeuxayp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3jovrsmzl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3tlarujok.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zacnhgfm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3dwfecxnf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3avgodlsv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ijvnhwep.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3zacwuhhn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3bshjupbq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mebhxmff.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mnchnfzi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nzkqnxpf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3mymivben.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3bgbkehwi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3juumjvcg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jepykhud.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bborcyxj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dljwjcsh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qormnlke.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3jqaknjzr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3kjxgsxwe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fqzyxtbv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3geadahra.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3rotepwyj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3zorrgqci.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3oqqjsjod.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ynfkkkid.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mpbyxdyt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gokjkzjr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3wvhgsxdf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pfaoztiw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3zxpumrvw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pdudphah.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vmyargve.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fghknwps.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3arjmprgs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3kthkrpir.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zaepkahi.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ysxdoymo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3xbufkwgs.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3trwhifqf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nwxzuzqx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3isrgdrmc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bigtdhan.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jjzeiefc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jmzjjhtb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3qoyigxjd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3linyvmtu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bkbumzpu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3icefzimi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iqredsgr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3stsefdhd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zeicvhda.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qemfiboq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3podeimcq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xqokyszy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gvvqhfus.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gqgbozpw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3cjphkqly.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3kthqebtk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ulmutbom.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jhxngoux.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nmliemwl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ccuznopb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wtzsypgt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3kpimgmrs.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3yevmnpix.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3sectgbod.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rheuawbz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3efrtoual.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gybmmzrk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3aylmgwvt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3fnznoygo.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ttcmoggg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jqtwevzs.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3czpdtzqc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3nhiozyhk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bgeacvoy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ttpjbuac.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eidihowa.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3lrqasbtn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ecgrxuus.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nsboufet.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3agwmmbuj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3epzkrmwh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3hanhvzue.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ikffrhdc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3hxdokgqi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mxuyeyex.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3sjvsceqn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nrtvurhf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3uqsxlcrg.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3cdnxcxvr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jnhcgkts.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3knfnohvf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3yubbbwef.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3kzimovqs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3tavwihyg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ndgusirc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3kdwlifos.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ilnlkzdf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3hdviuolr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3hbxkknjf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3jfidqvng.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3uzxyzbnk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nyryhldx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3uzaxmzwj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3grlamhnb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3vhorltky.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3kgujkgub.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3lzymmfgm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3nwtxbqmc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3rikpllrc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3mcgsddyc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ingjhhet.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cchtupla.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cwaqkemd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3durordad.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bbkrhwop.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3foxxjlne.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uhvxuxbf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3tfoypgrx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wvtoheym.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3jpveisyu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3lyhyaknf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3uxvcmppr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sdjcsegy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3cbcudeaw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ltrlieec.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3hwjzvlrq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vadzhedt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3jdiojdwi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wmaanmgf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zysxmbye.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3iofavbyl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3czsnxfnc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qeuivhng.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3utuwdqpx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ltnjwedd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ddnyokut.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3mgodqcio.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3erdblqtr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3borbhugs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ntyqsbgj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3urwdokmd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3yxzklvxv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ehbflsic.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3xgxtdgbv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zsbrjufv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3cgwqpuxs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cpnhskbq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zlbjyjlc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3twwzsyot.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lsygszds.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3yolowwef.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ygxvylwv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3biflfwoy.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3yaurohqn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vgqbtiqs.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nrsilils.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tdrcbttg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jjrrreyo.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3usmawlnz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wqqalkos.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rdchqccy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mrwlsrwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lubhuggj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3oysiaqrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sroprnlf.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3buhrhtyj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3jrvxgsxb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3emhnefbg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pyubmerq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3gxvddkmi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3zxjnkjlf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3buxwzqde.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qndcpvtg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pjdtzcdd.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fasaxtmv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fowtrwqh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ockmbnux.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bzljihbv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hytfamgn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ojgatntv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3yqotapap.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hzrnvvre.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3lfwwxajv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dhnxnguc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ocyxrnbh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gmwnylkc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3djctcdma.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yhcqneqi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jelvurpi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fvppxsrk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3npmzgbuk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3vbljgelj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3qqvjbszv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lsdmhlps.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3jbpkydrc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ihhaatkv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dqyxbhjj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vvkblqzt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3qftgrsne.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3riwmyqsk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uugayczx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3imywloxm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3djwqtrqd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3yrqguszp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3axtiylyl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3wocubqnu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qthccmnx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3udwptsue.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3gbyfpqbm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3szvtmaaq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3fawxhryd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hvhufceg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jwqubuis.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uxzvpzyz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lanhcauw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tdbynwmh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ekuhmlrr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3itxmhfuq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wnymeuvh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3smmrvmqv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3kxjwnnio.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3whafwrfx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3aepjtbkw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ofcrfqyc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3csppfbqy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3vkjluuhv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3bhmjhppt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3gjbadyvj.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3boxhrmfj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3hslebewi.html


<!-- 参考信息 -->