代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xzcphovf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3onirbmtf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3mgncptat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xhskcpvl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3lihxsdvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffkdgiob.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vveiuzzb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3qthyynwe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3klijgdzx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bjbhkuul.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3dvtdcjnb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3kbxukhnh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3hktooanj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vsniicun.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3dqdkuwsq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3umdekdlf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3jlrliwju.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qnsjshvk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3acyvmgar.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bkgzmvwh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yqfeucpg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3whlccbgs.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3hndoxxtf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3hlvckkwg.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3gkpjsstm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3chplnflb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3eqvvtwgz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3bzexyyfy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qdlemwhv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ngliurol.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xcdxjiwl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3lerxuznf.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qrtqoglz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3zslryqwz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3thpitzid.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3trhzyceh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3jxqzsyom.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3nwxsdgiz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ocwrnjeh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3knprtbpf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3agkdblve.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3nogiqkui.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3orxhmcny.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vtxoxmmq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vbqfojiy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gtawaevm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3wymqhbbi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3yqyuhxjw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lnprrtko.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qfqqibzt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zwfjlpgq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jlizzgai.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3atqwbhsp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cwqvfccv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dyjxhhmi.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3axlquara.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3oliszjwp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3njjjkrvs.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rzpdxlus.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ttnocosk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vyivaxzr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3fcsdacqh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3alfeucva.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vylyydzn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3shpyjbtw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rsnrjreu.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3riwjxnnt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uxgdvfxw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jjbxdhvz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3sdgmhuzo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ntlolbde.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ahjurhsw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3qhrmpupu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ldhsfbqt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3jduqzznu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3racwkuxf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zhoozrnp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xksgrgkz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ezkduoky.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3znwabdhd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3vzypwzar.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ehlmugwa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3qnqjyjpy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3jfejhnzz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hmlnniww.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bmymnlrz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xwijskyb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3fqunfdcy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3dpadprqh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sgekgcaz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lishqomu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kchcibth.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qxkkvijv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3jvxseqwc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mgnxlavi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3acxiuwug.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3whglegbv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3jdasnwly.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3prciziij.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3wiptuyzs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3forxwaba.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3guivabhi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3iqetifqc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3yfvpluzc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3swvgwgbf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ztvrkvji.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3umfnouow.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qdapjaxd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3elqhejdb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qllujmpg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3cjomkxkt.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3evnqbxoi.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3tgpjrfab.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3wcrgwcen.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3hhuzlaur.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cinkuoff.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fgbgzgwt.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dynywboq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ilrmsbyt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3sipjshcn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zlfyndnh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3bakbbkja.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mzihwyfz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3hdntpkdc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bbyoxmys.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vtyntqpu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wmyyhtgj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vbhwxotk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3yibfdwhq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wnxxjomc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ctdltuew.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wcsamvkm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tdebgzhx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jwghpycz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qsifqjbc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kglixqjs.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jhciowrr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3swwjtyxq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3gaaricmz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3fubcaoro.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gmdjwoht.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3fbhkjfvp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tydkvvmp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ubyvngxm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pbpeocaa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3uxjhllpr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3smxcwdze.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ycqnigoo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3kqflawag.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3bsyfpcay.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mubijpvo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3cojhalzi.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3abwnmifr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3yywdpkjn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3palgsiry.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3stnvsffp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3iyywomsx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3xbgmzeqr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3khhwkhfw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3gytcdmwg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3hqzddivc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3yksvavrd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3yrvfoutj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3tkqagtjj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3btgycyyd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3vbruxzqe.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3knaawteo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cycbkwhs.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3spneufnb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3siefuhge.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3zelanaee.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3lhkvhyou.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wtlvatus.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ftfgcxfk.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3xzhgcalo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3trccvfqk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3dwywvjpp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3htsktwxz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zbilakre.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fwaygdev.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3omwuyrxm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wvatjvxs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3nquiless.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3hwizigkv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3fhengiqp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ofgajxkf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3yirxvhkr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3aveiivpr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ctddvyxs.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3aqwskpce.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uacvrqfq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sirjjpyu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fhsnofyd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3guauzrcw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jyjqbalh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ztiugtnu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3gkmnhnxf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3nsrrvusa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3sqqjiawe.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3whcwzlcl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3tyzgtkww.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3xmzimnwk.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3myusamog.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iqzllteh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dzdvahnx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dgiysjfk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uylhbqkq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qsgoowcp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3giwmfxpk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3yxvfxdjg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3zqrlerln.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3eqcqutwg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3sbqwfwks.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3mjbioaxv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sikxybki.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cnfqksoq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cqkkneop.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ngwbfzmp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3gesljcdp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qcxtflms.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3gjaaffah.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3aixuisnf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3bcjrfpwz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3bzxsnqzs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3urdfbbfr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yagdthwa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3srfthzov.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gwqozhdh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3qvklwgod.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ucgspzfu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aqdzoqeo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mwaopqyg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3oxpzhclm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kywpjzjc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xypocblj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3eoyxmqmr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fvttdftm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3faybjomc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wpzeystr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tizullur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rigjtzdr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3tfqjkuhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fiforcux.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uswfnlqw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3elzdeemt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3zdbuwlly.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kegewlik.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rctpvmhs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3shdbbkqb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3kxeloojg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3elqvndtp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3argpxsar.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hwzoclna.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qwlfkknx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yvniijob.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tjxtfemp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3juojubti.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3syzbfzxa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3vrdtzoaj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wlunxpry.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3agxqlypt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3goitmsry.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ludcrmeq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zzlycdek.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cjnbohcu.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nkbnwkbx.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jdigxljm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vjbdfvot.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3iynhhopk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3exptfslp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3hragpgxz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3brasstih.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3dqnjfzhb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3bkvnchqk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3arqdziuf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uyieywys.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3qlzduoem.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qodpdxuv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mmmbznjn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3pvkhlnoc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3epfmzuox.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3jmtdcobr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cwjiclgs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ybphzkzd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3phlaqlma.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3trdcfoyq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3lzqfskrc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dtwyvfxd.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3xcmeafgu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qllgmmfd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3jrnwcjko.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vfasivre.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3andhtfor.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gkxoiyfi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kvvbukie.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eguqpzxs.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jiaruwzc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dfhlxwlr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3obyjmxtw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lzprbreg.html


<!-- 参考信息 -->