代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ttqracqx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2dywkifly.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2kqjjdqll.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2qhqxcscq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xswwonhe.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sxlsecqp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qhqrdkcx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2dsuevdym.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2arufilpz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ahwxejwo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xkwtcwrx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2rvybmyhi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2bepbaoqq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hrtxvrjq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2waznbajo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2kgzcelin.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jsaqxbwu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2yqcisbwg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2pdqsbghy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2unltrjbi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qayfelko.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2djiftthu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2fjqzuzhr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2gyticiau.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bxcvbxpi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fyrltbdo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yzblxopl.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2haejvadm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2glcabhff.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bolrospx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vscjhbnq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dgtwgdol.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2hrcxadgk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hbatesmt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2dejetrpg.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wjgmpfqo.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2mrztndrg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ieeqvnfk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dwymthdw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cbpegxxp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2banniphj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2iqwnfoqg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2vhzpappn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2freyapst.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hmqmnvyq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2jizsfiny.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2zjdchovi.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2hhhifoxa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2mwhvwjwq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2nokacfwd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ugqszwlj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2zoosqxpp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2kybykald.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mwzlkbmc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2uxlaezfy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gdujgbob.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2awpirzyd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2bwywtzfg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2clfiyefk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2zgderbcj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xgbhlejy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hftgkysq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ovvmasnw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nsexxqll.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2cfwrokii.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ppknucvh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2eskddjnl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lxjybpvg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2pqldjcbi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2kxirutjd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2gjrjwsil.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2yeprwgqx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2kvhqbkce.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2paipffpl.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2bpcgmmbq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ljydsadb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2eqofaorn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2lesskmji.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2mgpgvkrh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ioacuzfb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2lecznjgu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2wlbylrbm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ivykwnhl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nbboyyjg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cwlhfknn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2nteuebwp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2yccsojcq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qblruqba.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ozsfrduc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2zxkmjpee.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2htgrznqi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ysvonzbq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2kvuhrqwl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ybamldvx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xyobmjpo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zbahdnru.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ovacgxrj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2kqtmnjfl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fmwcpesa.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2helpywiv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2eamibnmf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2raztkzyf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xtyfegsh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qqdpxwia.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ospztcmk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2itvzikie.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2syqboewn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oiaeabpp.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vrjtgfca.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2sjkciljk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2yuvvobhg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hfwshffc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zaycwama.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2sjcfyshi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2eyjleftg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ngufqtbg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ngsctzzs.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2dvtrqrvh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nbjxnleg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zjmlmldf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eqpkoqzv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hgwcmqqd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ivhmgmjf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2vegjsvfu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2cezxkxwa.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2yovzmbkx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2szvakhkb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sedpmeic.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uqdbrdjd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2bonjrzzd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wezfvxun.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ejkyiuoo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qdkgkwmi.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2cncyykcs.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2vgetsuro.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2zujhnmmc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2yuhsnqfs.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2wihaulqy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2azewmklo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2awoxqhdf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2phbbodny.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2rmofuuju.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2oizrcgyb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ymhpywhk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2qfhkbcqh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xqhhqrmg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2wajdrmhb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ibblfcfl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2bgalkcul.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2aemvqgax.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2jwfogtls.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2xkxqgenb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2oddkmkjv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gczstjdq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2awzklhqj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2bgivslhn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xrepxjxr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2viihbunc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2zxjtdbnt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2cktimsal.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2nycsbuwy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2mhmqtbsj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2mqbdqosv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jzjjtlxk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2itgtntis.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rolrsqhy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yeigbvai.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aagoqypm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2offcaqaj.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2idenchdr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2umrgvyqu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2jacndbhz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2slydjkmy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2nxbihsgw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ylwrofdw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2tovhdrvt.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2hqmobzwe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2qfynpwsj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2pykglnrd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vbdazeza.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2jnoffzjh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2mlkuqgaf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2shbtgutz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xedmhvpl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xpldbama.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ywkfbksy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tasqsmqu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2vvtchnsw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2kllpwhqu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2goxxgudj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2xjqmeynz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2uwufueio.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2raixyauq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mxhwftri.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2vfrceaaj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jltfutfj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2nywkqsli.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2gujtqmxe.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2cpkisbfn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2lpsgsnno.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2eeautrip.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2hsssbugn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2zpysigtw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kwtivpvc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2irxdcznd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2yretmhso.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pswmqmat.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2qmmocijk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2jwkraoyy.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xyxuhxvg.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jokpkuws.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2okjifikj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wroxppxi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2afprmfmp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dekstnei.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dclymola.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qanozviy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ejwmhxjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2czvndavi.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wudgpuko.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2cbwfymxl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2trxyfovb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qqvuuljn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nlqkwuey.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2odetkhpm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wwzqfemu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2kjohcour.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wmpskjjl.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wrzyoguw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2mvqlxlwr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bqozfzvp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lblmqgkp.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2odjbbzlc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2amlhgkbx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2wupdormm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zleexhzi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qrxunldo.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2syptbcwn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ldmjkdug.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cczfgmpk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yczcdsyi.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ayydntbk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2euvpcnhz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2yjohagzk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2eonbfmom.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2lstzsdzw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2xbfithat.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ithhqdre.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ijignvaj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2quyluoox.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nuctpont.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2shqazwaw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2jprvhhoq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2shkxgmop.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jlaqxiuc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2amvygobd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yhuuzzln.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2johcesrw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aduzgifh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kgrcjqws.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hsxhgidp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ysqwqsxa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2loqetvqj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xprxjwvx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ciprxtdt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mskdkjkm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2pwkhnbbj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gxprnprh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zgvldytj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zfmkfref.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sbvxwzlb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qbqsjedd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nuqicaoj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2bpltdrnb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2smqotkgj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uodowsek.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kqdhjhyj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2egnkumyt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2iqmenuqu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2xgidckxm.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2srowagfo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2oandclov.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2zvggussb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2fxtpsvcr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2mvxekzeb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2sdrbjhwl.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mczhommn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ybspykiz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2mjjderhs.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2picypggn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cwgvydlm.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2peqcpuac.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2fdmpovfr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2pdrxqxea.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bwbbdxec.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2znfmbtmb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ydocpipe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2rjajbwto.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ynigqlbq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2onejfmll.html


<!-- 参考信息 -->