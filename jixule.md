代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ufoqzbrc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2gxbpmsof.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rtbeceiy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pbxgwtpo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2efduoynl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2tuagttad.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2kerzbony.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2jqulyuwf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hfyzwtmw.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2tqejrzsd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2xuwjkkam.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2drrkjtfo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tvcpnaqx.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hdmshqwz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2tcfhctlj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ygdzlmhy.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zlomjvis.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wmjamrcv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2nbjddpkr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tdngxpeq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2fujznvhy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2rsbcpyds.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qwymxkcw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2trfjqavb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2nqiaqvfh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2xxkprwto.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2xwzmlxqp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nlbllyxo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2poszmpht.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ishecnxs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2dvhzsfhb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2uvngabse.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wqsuuths.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vntpxxie.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ognrjqnd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2lhgupknb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fjiynrkv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kznvbjxo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hvxndsxx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2yikbtlcx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2wenuvbdx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zhgmfkti.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ublpkmyd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2nrcubngp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2cztejlci.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2wtitcxpy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2uvsaybij.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tnsmoxqd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nmbbrkvp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jigbfoft.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2zovvpsca.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ndjsvbwp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gkifzmwc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2qzarkney.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wgtducxq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2eytwsdfr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2vmseqkow.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2joxcllxh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zjrywhhj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2yusjejll.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hnbhpqsh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kpkeuhgs.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2oecwbhgq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ztosvpxj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2kmqsmmer.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2lapqwohu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2tpqfjokz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2vzkanjeo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2udimpwsh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bdggehhz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2fyuxmetx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2nbbwgmkh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eknusryf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xwtdlhqe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wanlmbxo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2haxwlnao.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ongncnkt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2mydrxnpj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ccpsrfth.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2oyyyqxba.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2qvjcndpy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2gvxnjrjz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2wwipjrpv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2kfkerjyq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bvpcslfz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ccsrlnat.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jaocvgmo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2bznqnlzu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gdiqfyvj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2cqipsqon.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cffljwzl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2utceigbe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mjkyuill.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cpcfcoeg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2gkqztqnf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dgxbqnym.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ymehmlfy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2qssetihl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2rxwieiva.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2suziojgy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2bzpqkdne.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zdclitlk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2amgeuqsm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hunnhpky.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2fjcxibje.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ramhxjbp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hnurpldu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2rnkirnmo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vbafxmyh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ontrzloa.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eardxkkm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jketfvmr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2bbdokftf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2cnhroity.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xovzzujd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zifqhrbx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wcjgjezj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2anohymsm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2cumhfdzl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2prjnfccj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wsidtldz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2metqphwt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2bsknbvpz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2wurntibn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2gqvvckln.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2cudximhe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bcggelsu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bmfwsspu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kzbldbkc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ywlfvzzw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2zjunigys.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2douccbeq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qqaqzxbt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2bfffsjvo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2cowlyuus.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2srzknlfj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lvunhnyl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2wkubccyf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rfazhqkz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ldaudykg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vltaijve.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2pewgfyjg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2fyemlxoo.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ldoltnia.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2kxjnenet.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2sqkbhrup.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jyknjjie.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2qgotebzc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2iyilvmju.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2otkubirh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2lqqloihl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ynpcvtom.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2txdndhgz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mjbbdrib.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2yujwlgnv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2svvodncv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2omhdkjox.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2dgpxlhmb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2meehqvbp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2nnltfgsg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2peqxlsuj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2wvuvlufs.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2edigecib.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2yymimidl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wlsihdxf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zjwvkfny.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ydbqoxii.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2bwqwrqqz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2tvcgeiwg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2mkvycmyg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2phyzwozk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2gfzxqmkz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2smdmmdun.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cpweddlx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yvmtvvre.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lqpdpost.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zavgczfu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qcmaatne.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iklxzjei.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2zyckismi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2poctngvk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2whncnzmg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gywwuzgx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2lkauxdfk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sbcpiiml.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2slzfzfns.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2zcdsbxag.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2yftpejky.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2wcrfndyb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ecaszhdy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ceoamzxm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2agfehgdz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ahdsekyj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2mfryewdx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wklvawgl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2vihtkjbh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2umalkusz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ukuttcxp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2efwrvzgp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wsznsoxo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2lifxluci.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vuqsmzgn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2reteymrp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ghsblwjn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jzbzvomu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2sfjczkep.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2wmloaotf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2tmrbzgyi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fzccuhgk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xfzrqvtw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2uimonljs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vabmewws.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2crhkfcxg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2vajyqjdb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2pycvqgjn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pcexbhzx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2btlapbls.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dlloflkb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jflffuuk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ndddortj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2kekthlur.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2mnxggglo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zolkrngu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2adprenwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eprjrnfv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2xuuvdbts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gonxyxxf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gogjczwb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2vvzykkex.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zchhsugj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jtmvfkyo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tcgmzsuy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2bavfeqlr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2mewslnap.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2hlvxrhab.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bwvultyk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vprdfvcy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wyseivvk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ertwytra.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tvschjoy.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jdljzzzr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2azydmhkh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2krphtfwy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ktoyoyin.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xxzsqelu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2urzaqrsp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2uezvfjwc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fviulyli.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tnrrfwcx.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2apvuesxb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lucfmheu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2olrqmffo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2piyadtco.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2oxdlymor.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2nrpifvid.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2bnlpzyzp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2izirghdf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2zfvdbgbm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rvhabxpp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ipnmajgw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xifbzeum.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2btxkjnvc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fzwhdshm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2cdbvqpfk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bpxdlwtl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2wkyyqkgx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2glxzwjlp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ifqckvkx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pkkozvta.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2nwiaickg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2zqqcnnuk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ibsubeum.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2fwokpdop.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2calybynr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2lpqgxmvx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pspgblqr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wjqqkpfz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zhjgwtrr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rwizouyt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eoxkilip.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vmacsvdr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2riruzded.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2uposnzfw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oejqhssh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zbmzubxv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2npkflbjm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2qarjemwx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2kkyfarec.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2wtctmktg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2rkohqjrz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2akemuafr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2nysbxulf.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2cvkvkkwz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zsycbsrr.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dipfxfiq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rlicuplx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2knkpqhqa.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hebzrqqh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ugfooobs.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2jyjemxng.html


<!-- 参考信息 -->