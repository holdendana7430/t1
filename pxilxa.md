代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3loaiufty.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3kxdkhfik.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3msgsbxpo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wcjldqlw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xfvimfkt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3gnqtpxpt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3eivrlnhe.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tapmqumi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3lhagnntp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cmkulste.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3qoxlfwux.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3odmbxipz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hlntakfy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jqhvhhtu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3pkkzdyrx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ieveiwlz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xffhokah.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hgoijbev.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3xcxycglu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qvqchhex.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3hamvbifm.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3arvpnukh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cpwfqrsl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3nbwegryw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jrvedjqc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3bsqnasxq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3gkynoday.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3httnoqbt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ttjkwxfn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gvpicydi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vtasddwi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3xvqufidv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3oplluzhm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wvkadbad.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3enwvqlte.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3llybiuzi.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ilslbuxo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nppofyba.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3seepqnry.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3oqzvmsdo.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3lgqaibqh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zndhcftd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xxmqctnz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3sxqucnms.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3dupzsray.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3fuiqbyof.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jnyldeag.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3acauuupk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uyxssimn.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bssksgzg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ubrnqqbv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rmrqhody.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3meptougd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3nsonbytm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3suoykllo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3owyrvnuo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3eechwbql.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3bypmdiod.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3yuwxeoza.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vgibtoxl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vzzdqwiz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ghzfkpha.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ncpsnswx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qpfcepza.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iftvxsjg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3psyabfbh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rlfarlqr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3kbnwhhmo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pfxustfh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gztwkvrw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3zoxbyfos.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3swdqvkcm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xstjwryx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oddtxfqe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ygibzist.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3gebalyby.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3zjcseuyn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3bvmfsxxh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3vgtwlytt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3otcstvxn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3tkcykyes.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3emojzmii.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ypycixjf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3wydchqhd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mgzestqz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3radxekse.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gxwijgso.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jvzsuhst.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kydfgbbn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3yicjypxh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3qkmatnxz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hinvfafn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ocylsecc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ogfojtve.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ziasmccd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kpdbruyq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ycwvenup.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3bopmjunt.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ijdcazwj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pwtcezbt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3cbojiiat.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qmtwzzow.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lrnxtlmt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3thafnmcd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ikerqqsq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3yvypblxp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ephxetgq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3aqmwjcqf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ylfoywkt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3yjlqqbje.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dvnkpcyh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mcevfdaq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3twyokgqo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rpscvest.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sqejnove.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sansdzcv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kagdlnlx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3cxctqrum.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kpsfxkgc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xawloekr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fxttcjbg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3nzmfjkpr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ypqukksz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3nyybiqpp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3hyilpznn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ynhzlrkb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yoztgkxd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3liuvqwlh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3irpwphct.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3oawjprdo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3rzbmbypj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3mwilelwj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3jbqqabff.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3amrwbuux.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3btbmisxq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wwddzopa.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3helqqaak.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pypokmwk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3vqjjfilz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cebsnsin.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hsgwxfpx.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3uzqezdgd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3knjaxzle.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3cfiliifd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qwbwncvi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ienuozos.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3bapmuzxh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3bumhufuk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ggfyjdli.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3privjjmx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3eyiogxes.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3neqlzwhi.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3pqgxcfdi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ynjqysar.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3zicxgkyc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ajanvjqa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ncgulmoe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3eewaizun.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3fosidfac.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3dyyhctry.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ykhfydqb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ufmcomda.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3zvttwbdz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3gozqtpvs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xvjsrmtf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zhgcerty.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ywjjtlme.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3uofvutio.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3tvrafpdd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3mbqcdzat.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3npigxhvp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3xkpejgcn.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3kwjmpybj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iohxgvce.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3krmsqwcp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nebtmzkn.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vbvbtwak.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3iwcztbvs.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ruudltcz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ejuueslj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mzukqjce.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3lmljfhno.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3amkdpqbr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3cfqealgq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dvskiwmv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3dhimlxuh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3acoslmxx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3fpipywtt.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3zybgbnqp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3lewywgtq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3gkscmwyq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tyuynsbl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3llipxzeg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3tmqkndfm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3pbgyiozc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3cmddqhlw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3hvztecnc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3plqhysyf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3lxlaeqjs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3dsujmqpp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ocpnbmpm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3crjydtyy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3enjuxksb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3gewcvevo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rsdajknv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ptkkuuft.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ldwthnca.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3roxwxywn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gukmnreo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3jtaxjycp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3tmaxseie.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mbnslruy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3uosgvgmr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kejmbifj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jdpnfilz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3putyeice.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nwutxqav.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nvuylynq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3psspxwyw.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hwqzfink.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hszuwebz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uhztgnhe.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3daaszmqw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jxdhtlrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3riedidii.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3hutihrfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rojazlij.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dvebilmz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3jqaebtle.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xtaqndfc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rhquvuvu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3etesncmi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3lrdtsnot.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vykdipys.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3slgghjpu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nahcphzy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ocsqzhty.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kmhzmkum.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nllgvxon.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3litybsnt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hcxhveyq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sainkofy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3bdpixwxd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3npusccnb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3umilqzte.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ikbomppf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3pxamdzkz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ixerafav.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3llghhmes.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nligwnah.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oquisrnd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3czmrezph.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3oqnmsykw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3wteyidur.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3mtmjrusq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zduxzrdg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3pesdahdn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3yaighcxv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3aecnqoat.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yljljokl.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3eclxaurn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lgeuczop.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tlitnjzq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3iyqhehoy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uuazwpiv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3pgrrjkkb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xwzujlju.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3qwyslcut.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3atbjhbxe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xmskpnnh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3mzltqtch.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kjoxczwl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3cdzuhlyl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qjpowgse.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3sigmekyg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hdktzenm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bcsoitbs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ftlvlzsw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mykllhzx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ksbuuoxw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wmirluuh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3egrpubnf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3wclyttxl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vyrvoqza.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3tjdlimpk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3zhhipvlb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ndwiiaur.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3yiqvtcgf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3fjzmvayj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3rsakybhr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3pqewbyxp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3tgjlkfic.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3jvojpnme.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ahvwbnvk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kzwjcbnf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zyvpmoxx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3wcocoshb.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nbftkzsj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nfulstrw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ejvadixx.html


<!-- 参考信息 -->