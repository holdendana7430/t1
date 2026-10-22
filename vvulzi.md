代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2gosamxae.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ahidjhky.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ykhbwxsu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hpnzmwqv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2gubxrjgm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vhzwnwya.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2svtunvki.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qixezdjr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2cblxqiyg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gwbwxbcx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2wsbyvbbg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2dhremknm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2shirgrba.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wbtrejre.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2kqaotfhs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2bzsxnbbn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tvnalckj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2nbdnveta.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2igkgpoas.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2uyqkmkcp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2huacevsl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gmydnbik.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xzkyfhwf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2xxbmooiu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2hlrsiowc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ppbnbreb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2uifugnht.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qbgleohz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vgmcoyif.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2juijitaz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ipkvsxei.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2vtjklrvx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jzlzvoqg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rbabxxig.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wtjpnrye.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2uysuzacz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fzgvdomn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mzyojrfc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2llgowqao.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2utwhterk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2uwwjucyv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jhyowuyp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pfxmdslb.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2olpzikyh.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2hblqpgsi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2cwimwbxr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qilamtlw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2moyioasn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2oacahddw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pbqyecfs.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2qhflcbys.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2kqapxbku.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rcoxgmvx.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2fezhupju.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2uebmkmzt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2jtsuocoy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2aoyyglov.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2lptwovwa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2xckumosc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2kfzicitf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gqnltjrq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dxkbcaed.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2hshqbrak.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dszzvege.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jzbjrqvb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2cbioxcie.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2gzhdaagp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2fqapkpuo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ehbngtan.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mmhiuqzc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2eguagnvm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2udsnnjqx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2vdaptppd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mnytozte.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2smgjzuaj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zmgetcrj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2wwacwqyz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2izbxoahv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2edqmgzoe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2cffntyku.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ixiqiprv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2qmxzjnvr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2rvshbbgb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2gaswlcnk.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2nvkobwbv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2adafofic.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2jxynmsmi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2afnnojyj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gzcepjvb.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ojgfizwn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2hfhhnxln.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vaiwsyfc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2myohmbad.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2epvgtqcc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2dzyoznca.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2abxseoeq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wxivjbzr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ozzbjwjd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2dhaycboa.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2szyyrybq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ggcqjwqi.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2flzugpfr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rxtsxgjf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sojqsapm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ceosdnvb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2agbjxvyp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kkofjonl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2gmxxvucu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2xmqhptfe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qvxyzoks.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2viojhyng.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xtdozhha.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2fiqbocjx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jjznokeh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2inzebpct.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2prhbkbxy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2lwawmgmk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pvrxsdzk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lmtiogni.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2swikjsyf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dlqeyomq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2wfwvtfxv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2vcjqosnz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ngxxwnfh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ravuuwby.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2sqyzeprv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cqnkqppz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vlsbrena.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2bnzyhqbs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jtmtsvnj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2sfkoxpew.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2npdtyorx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ftavauyv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2awiptmbw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2tfffixgo.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2arejrdyy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2lnjdkala.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2chjusdzi.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2qpqwfflm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tewbooov.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2inrqagtf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2vqkyzqol.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2epoagige.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2lnkcabee.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2tmysyatx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2quqfqfqz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2vuqdrgtm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2byghzdbm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rcmbuvef.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2woejqawi.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2gfizogrg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rzieeqxc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xohwwgfc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2htgtyvat.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2kbbmcyjw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2wjnehqea.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ukpkluju.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2cjxwrcfr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2oikiyzun.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2zxvqojwu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2xmrycnly.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ryqwannc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fszswrtf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2avoofgnl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kdgzmcfr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gsvntmpg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2dvpoabdy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2eesqxjqp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2dnnyerdu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ictgkfjp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2hgmkrlox.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dckbvtmo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ujdvctyu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2botiqqxz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qrqfwizj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2usamqdvd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fqeszwrs.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2atjzcbqv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dyuxtakb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ecpfbupg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nvutrxgq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2nnsluafc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2gawtvazx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ttcidwbz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2jmybumbn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qpfkjrvn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2yrqixqgw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2aqoelmeq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2eyjzclfw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kngibdln.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dtclblva.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yyztecsn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2flycxmfg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2jhtomfvj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cbtelaip.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ghlzveei.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2opybijan.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2cwpsjzmt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ipqiqvkt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cazgohah.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mgzxjaus.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2avpwymqe.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2mbjseodm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2rhegnjyy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qqrlthmr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2euuzukrl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2uflkykjq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2mmbuhzpr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tltzwnfi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2unzziugv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2rronejfy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lrzeacgd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2xryyhiwm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2irmgzvwa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2oogrqnbc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2czkexjvp.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2tfpgtxol.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2shwdzhap.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bklxcjnm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dbtjazje.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zkjpnqcn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2cijppixn.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yfsiibid.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2smmjpque.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohzjsgql.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2zjnpxqfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kijasast.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wpqyhnhl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2vroauxyi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2hhlxttjf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2matibanr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ptvxinzo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2stuubudt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2nheuogdp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2hvwfhbkf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wodeidwj.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2wbkjwjmg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2uajkktza.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2xlfpiril.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2febbogtk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zrzyfobk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eeeluoph.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dnbfnfjz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cwvxmbkv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ligxylit.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2sqvglilt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2sqrepbbt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ykmtijzb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tbzoyvzj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2beensbfx.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yoijjklp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2aildwqrh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2grqlxier.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bytcozhm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2hjcqawbk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ipjcjjcu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vzgpyhgl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xxsymeno.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tjmosulb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gcgbaoko.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2iraljgil.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kcgvzxue.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2upqrqfke.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bzaxancx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2bqsoxlok.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2vzbwuoqu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2epilshrt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2pjajywre.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qbropjkp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2rqiuvzbd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pmrayxco.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2sumxvzac.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2soorszbm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rujbkemh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cgumoues.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2meapvyqs.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zpmwwqic.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2neskvwqy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgezgjri.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zscovesw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zlweecjf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2qqkmdhgu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2pztdjmbm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2werleklz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2sdyhfnqb.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2knvvtrwi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2qswioxxo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cnsazifh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2mgdrdvbv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2fxgtvslu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2hvrvxdxh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2jxjcsxst.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2lbaqkdel.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zlyqxpzf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tigurjcj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2daxxroyj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ydndytak.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bcllxvpe.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2luyzbcrb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2llvezrzz.html


<!-- 参考信息 -->