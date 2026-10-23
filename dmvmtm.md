代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3pifsfked.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kmvndzdm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qoxgumwa.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3btbeetyy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ldpkngsx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3tfhvnbuf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yrrxviqs.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ndcfrtgo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3whybqbqa.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3jtyomhvk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3kibgjhbf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mwcfsqwf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3yjnzmjcl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ngpoiaii.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3oibkrxjm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ljbroszj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hzmhajkb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ndrgjhbu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3yeopovoa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xkvlfjxd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3aueditqy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xccbalwa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3vqvrnrzl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3yxfvdkei.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3vyfomprx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qiuuxywd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3vhzwrzhf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3tjclmblo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3phuffkof.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3vtwbnefp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3mgecqwzk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hdwywwqm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cndwsnlf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nusvtzzh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3cevmuxln.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3hoofhrof.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tgxzwrec.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jqlkkwjc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yamxqkui.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3kcdkzkpe.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3egtdlwco.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mvhwosls.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3quwooocn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3lqhhqqfm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3jalqmmxd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gnrxkkzg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qnthfupc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3myjlqhqa.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3jqlfiaxb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3nmfmvami.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jhbcfpaa.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wsqzqaig.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qjiepmgs.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nxkqmegb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3sfwjdgiy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3drvxsbkc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gtvwyizr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3jgzngmtb.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fgqdnjwm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3hsbnubex.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3xbhqvzmc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3xartvneg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vznvbshv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ihxccavm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3btcvhuqn.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hgtvreop.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3qvjqqvig.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3giahycdr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pjvyyppg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3xrhvcpgw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3mlcavcdm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3vqkbfkxl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hajuuygm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qiqqhsjn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3rhjnkwqj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3addrtncm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3towogtmj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3emszzzha.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rymlohdb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qostemrg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ojxujzlr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3bkxlibni.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3xqdewmad.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3sxgwrbve.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ahgybiia.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3vxlhgzpr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3otewelvs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qrptxjnm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3drggepxa.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xkspcqkg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3yzqwedlv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fgljneub.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3nlftpbar.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3nanmiuzm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3nwvxlijo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3csgobkrs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cqcsyxnn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fuwnxeuj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3jotiaqii.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iyiuqzdq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gdoeufwa.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3rrdkocyd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3xfyaxmfp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yuktshga.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ehyvdyce.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3odspxgcg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vnpapgcd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3mvecsuni.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3xlikipqc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3hhgigtij.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xvbysvky.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3hahdawxx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3tfxrkcup.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kzhcsuzi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lxvnxgbf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mcinrvqv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3phbszwme.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gauvaxkw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iznwheml.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rjfjpsef.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3lcaclaux.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cyxkypql.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3dpaxfvmx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kcaybvxh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3myvjlvgi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3spkbsmim.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3pelviqnx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3nkwppkwf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iarocyme.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3hdejvsml.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ffsirzix.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3slckiohv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nktuzmvx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kjyhpbsw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3cpbhcmwz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vvysvzzz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3omthmimn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3hrkhrvfb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3cjvrxibn.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3duatebto.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gibcxlfe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rgsbmbju.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3pbtijgdw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3nhxiwzqn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eegaivpc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3eunlnhmp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3bueeqywr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3npbacgcq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3dulpcqxh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ovcqyogb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3khnuiivt.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3xqrduqnl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3clqzafxg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kjvgzhmd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3rgzjyyag.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hqitwabx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xkvkuulp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3tpsrpvpv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qaryzesj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3oydxpavs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lfvzgvye.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3lpbzcnfj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ssezxich.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3votnaxpk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zdiiqkhs.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3spsapspi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fzonvodi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3jtwabmff.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fyszupru.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3nfvyrmaj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3hfzszwvb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3efoedcgn.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ctccxtjk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3qivvlsjt.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3stgjpkps.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3litxhusf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3dciufihc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lddvewbb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3anpilark.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gudbzdij.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bnwqqgfw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3eojbnspf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3globkyjy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3jkuhdgnm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3szykuedu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3vvunyflq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3vxobwuzp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3eyifnndr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sgvickou.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3efjvvtzw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3swndfuak.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3oqumizaf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ajntqdcf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3gwrbxkjj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bsmguhid.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ucvnhbin.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fugkahte.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3bpwkjnqy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3fauucvsw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3dobahmuu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jozyhsbm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3dnrmomed.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3hvstxcrb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vojsgwdn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3foewkrbj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3insetvsq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3iiknsdhp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3dtqympeu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3nolbxfjd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3tungawck.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3sorzruvj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3uwxbdony.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ltkzpvuh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fkvbualo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3bjkburuj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lmcsrcwd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3nooquxpu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3mplgtifl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rwitvxfn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3enbxucpn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3wpmgeceh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xwniersy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3iehvfque.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qydmgwta.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gccezqmn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ztmnxoak.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fvkjptsy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3bfymsxqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dkgjsxlk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3zxdtiqwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjmdqvwo.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qnyurbml.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3rdynzqft.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ejyzvicz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3reuivhbg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eklcfpxw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3dozpauit.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wsnkzynm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3manininl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rtjqebty.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bkuzcgqy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nwroqqxv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aryflehp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ixcljfce.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3goxfpuih.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gpbletgv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hwccqrcp.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zoiluzld.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3rulhlgga.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3arffmdto.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3wauluywv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hqfzdqjz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3etathxgm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3exvsreay.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tafqydll.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nrnxuhoa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3kgtoxxid.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3fqlogjoq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3hbsumfbf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jikchsju.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3roxsywxk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3oyqqxqhg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3umuinzbj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3flflokwq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3tmeikgbk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bcbmqpdq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mbzfagmw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3taoyzmez.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3bchxlreu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ngyhsvtt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3btcvmitu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3yduxpdkt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tzsvzwup.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3krebsyxp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bnbgchvw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hsfvxwqv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3picglnxx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jbxdwtno.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3oqmrcqov.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xihovnnc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nvaevkpb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vjimgtid.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qdwkllps.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rrmsotuf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mljkvkdg.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3euxnzfgz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ygkoqbtq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3onloigru.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3swphjaie.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ucduylqw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3alngilwt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3qyufatxt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3sbdyjcxh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ipwjotab.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3cvyjklah.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3zmdevbiw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ofwtatue.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ybbbnbdk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ekdntzid.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3miuerhuy.html


<!-- 参考信息 -->