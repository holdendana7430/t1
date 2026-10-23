代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3xqsphikg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3enyixfdp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oxaucguk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dfylzwze.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3dprxmbbi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3lqqzyrko.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qbteuyfo.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ohjwtdpr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ctevrulb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3fxbtvrbf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3dytnonbv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3mgdoaezv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mknlmeyc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lorhwarw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3wvhorawj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3bigkgagd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3djvtsrlp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3cygzvgiq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rxknbnlr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3slisydkz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3asqkexrc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3gtpfsqws.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3uvjpaxev.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3dpzhsvhy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3whxbfkwe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3kowzywon.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3xaeaheoy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mpklrrsp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uikuwofn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pmwthrak.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3dsyhdyno.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3sociszfw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zejtxzzp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3txfeegzr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jrqzcexb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3oyauttfk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vubfzxbk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rcnnqzzd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rqlpefpb.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3uuzgabac.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3lpmzpjhi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gjhegxti.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3pwaacoip.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3yopetqst.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3zesjsxjf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3vlcbmqcu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dvjrkjjk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3sqcveray.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kubncnxp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mjjfbump.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3awapbfel.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pdrozatn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ljwxzewv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3cimfrnrz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qovamvww.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3uicqzzlk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3axosrwcy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3mjxagmcl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zscujlst.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3lachlumq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3nqokhkad.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mogdslvy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3pgjddclj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3iobzvyfw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3qrqvuyar.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3grdidlez.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3xbapyzxv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mippmueq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ccchqjom.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ugjxbdiw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ifrlvgqh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3mfznxrnp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eloqsijn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gxziwtng.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vecitijx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3chladjkz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3tmdzhpel.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3hpbmhxzc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3qzflcpde.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3gbepfsrl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3oaiiadoc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3dkvwjbic.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bxsrefwi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ptgncyev.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3sodnipig.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3aigjgqsw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zfmpsmtz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3oiasgorz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gujebmmn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3wmrobapx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3kibfboae.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3czalstqz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bepthmzh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xckvvncb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3jddafwlm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mqlyufcb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3zqoynksc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qwqudtxn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3dgdullgr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3nqzoiifj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pjzrsouo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wolyvwhu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kzlhaowy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3sqsquter.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3mqtxcfnr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3gsirgjpp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lfxdbskn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3facvxxot.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3hudilwra.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3uxxpujyu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pfjjfutf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3anxvatak.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tuigvwkx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xizhcivi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qubiivnc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rwhsbfes.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3epnciyih.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sbrsozxh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lsbycovi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qnkyjhdz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yytiotwg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3shbpvrww.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3twniydwb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ezgylzji.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xdewdlrn.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3xpfvxavm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nrwzjydt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mtvcyxjv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3efgmzufb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3darqjkfu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3fljeeczv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3dqvsvsul.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xwauesiq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3pjxrtlco.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3lgbdgxgg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qtbpomax.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3kclwdkzl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mdxmdupr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3crkljyhf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cqyptkvn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eguqbbhl.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3xqqiwhnt.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ajzikepu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3zzaphffh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3rldadosu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3srkogrgv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3vuybkpbn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3oddpuzcx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lrzvdeen.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3pcaausbc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3pwibzpos.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ihlewqkx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3dexsytgz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3arcwsqcc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3jtnaoymv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ldmvxnka.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fsqrynfr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ixgpbxga.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3cyqdcfqm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3rfvpbjhc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3glgktczv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xakavokx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wbgbtqly.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ceuvcnib.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yltwdlte.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3atwyiygy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3coccggnt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3nsvxnpdn.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3yzqwvwnc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3dtmtasbz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3cgvqnfws.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3lphxvkby.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jewmiter.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yiolqglx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3apmvuojw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wqmfkzfo.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ncfafjum.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ansuovbi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zztobhhm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3awkbcvfd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hfqghcgh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3wsohathg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ggmvkexc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3fwpirutt.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3brmjqluz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3dbxsrlii.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ovooopaz.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ejnvmeho.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ztwfylzg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3kntldnod.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3hvswausd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ptkhgcpw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pamrvwaj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3msgsgjyt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3hiimnhux.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3suvineds.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3tgekznxh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3qkjccqmd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3voturlyt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pagtmndl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3zcmteukd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bsdnwckv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3euoafopb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3sclgbajt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uzxnalyz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3oibwitcs.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3twlumhgq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3bxljztci.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xictvqzm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fuonjbwj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3hhdosdeh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kdizsdtu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3mtwnznno.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3smrbblka.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3prslfxkv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3soxhqwdr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3qqttqpfm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fyiiahaf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ceaushfe.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ngzkhbzn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yiedogmo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3gipmctga.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bubdxhgt.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3snrzwdij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgxmnhdx.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3krvegjmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvaudmow.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mgcsabyr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3qfagtskr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ahtmrido.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3icvovjhu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fdsxtcze.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3opjfrdoj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3upuntntm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3tekzgquu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ggehfhhm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3vjypomif.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kxrofsvh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vmrlkzcn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xgovpziu.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gfzotrze.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vycnggwh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3eriuymxx.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3essncjoi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3yuqkouxb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kwtbupik.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3vpoeikyc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3psaqivli.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3brgixrxg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kdljkrii.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lqezbpcf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3sfxogeca.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3wbjsgkde.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aepqbqcp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3lnzwvtdd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bfzzvnoa.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3hmqhajof.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3qpwnrakt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3umjnldns.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uyybqpkk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3dkjazvch.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xminlfvz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3motomjtl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3cwhuggss.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xkeimbwb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3wvazojko.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vhrugmre.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3kzvomeaw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jdthhodp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ibkpoakh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ybomtupb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vyraikbg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3zhjzzdlc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3saanlewi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kepircdz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lfdzwpds.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vszzjmyy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yovkiwor.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aehlslhl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dqncxakb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oxqatmyq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3atsmzwjg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3rbajctzq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hspvfyem.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3evzriias.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vrjlwkph.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3wtgmxcdn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3urzzvptf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ucbxwzsc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3sfcwfwgi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3beggulcy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3yykvcczf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ithnvkyk.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hhxibkqc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3neexlxmw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zqrjhpad.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3wwvgdvjr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tzbnpmkz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xkmnzvhd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3poeelxsj.html


<!-- 参考信息 -->