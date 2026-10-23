代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3cohzdnsa.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rzkudtlh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3jicoczmh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3iljijvut.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3inwbpvqo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3odprzhch.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3miebvcsm.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tcypenqr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eehxcwkb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3teavzhps.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3qmgmoeum.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3hbszsana.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3jeijkuea.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xgfdvbtm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3gqrqtnzt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3eupofayz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vgqyrxsa.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cwqtyaxk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3rzlgxoil.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3nedutzla.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lqkwyitf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3oggfemgd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dqndjwzp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3vqgjtlqa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3pfzmhiyq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3uymvpzvf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wdhmenms.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3igxsewir.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3mdxjmnyt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ajtnzqqq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3yichimts.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tfktpqfr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pywgrvyt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jyhcyizb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3zeocnuaw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ckeqybot.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vxysriqf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ogvblckv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xsnnmmif.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3biizkmar.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kwefmylq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3roncbyge.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ppizzllk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xlilyhud.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3upvmpddi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tqustedq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3pwxhspbg.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3zdcxxwbw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ahcyietm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3mthiqzef.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dtuztarc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kcwaqivp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kdjlsrli.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rojtsvig.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3qjhqgqzw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qtxvbkjh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bmxbpgvj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3evssbacx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fdqmcuaw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3jetenjpc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3tmgswhyi.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3sxjjuhwv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ymttnnlw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3xahokqnt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3vxssznlj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rodqrnge.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3zwvgvocd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lmwvngtc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ysnwzybl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3iztomacc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3nuxfyzkc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3djlxeyad.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rvigektj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gytxpkvg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3izhqhuxm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3wtzsztcz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3przdujku.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rybgsqrb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3smevepyp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xvdddclb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3dapwxwlq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ftglgwyd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3lojdyzly.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3yfiqdtxp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3jztqesta.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3hdxengwj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3jzazxlil.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3epgshywo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zslqsygs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3lsmvtpwb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3csmeifam.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ydlxjtde.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mkljpbpa.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3hgqoqxqm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3bcnlrmqz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qverfuuz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vfhegbip.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qtdzgdko.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3aorvymoe.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yrvnbehc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3isbcojkj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3chgwmwdt.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3hmpvynhy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3qtgeklag.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ljvvedfh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jcyllcxn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3brvxtecs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gpcvqzxa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3pgutreip.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3menxolhc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3htjywpuu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3lcflmhbj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3myoejdos.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ivpyoacj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jkgwqkaz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yzhhhdrm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ilcczeua.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wmyrgmjy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yaaqepgq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mrvnwtbu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3uvvadpzj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mdtussqh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mejlbkws.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xurxwupu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mfygwkmo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ybtuquqr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3kxugjult.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ycnjxekn.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3riczscjw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3jsrclmbs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3irtnhjvv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zztbxrff.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ktehwcyw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3feslvoky.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3kjhoibto.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3mefojxlf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3uluqjzdd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3fjjtkmgr.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3qctouyrk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3yyfxjhnk.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ftixpher.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bulfildq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dqvcrtxt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3hgqevrkj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hrbsyzem.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3oehhjnkn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3mrhakfgw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3sbbupqrs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3tqhcjjsr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3sgdyxpkd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3nggvvkdx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ptjbveoo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3mjdkvwaw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3yzvoyucb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3jtglshxe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qkuotaks.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3hxgjtcyo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3vfhfcqop.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3uqphzaev.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ayvbdsgl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3bvilaxae.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3yobdfnxa.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3tmdywpdp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ejrfwazo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ebheubbq.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tezxewof.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3zpzhdonl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3irqmcuat.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jgmvblio.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ltjuhcok.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3dqpjkpgz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3daawpsps.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3zamcthnc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3cfobaxjq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ejhuqxyg.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3zypyzhyj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3apmimwbx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pgoqfdah.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xqaylooc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xqebbklw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vdvzrxrw.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hggqfhzy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yvaxokvw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3yuzhjade.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3elnrubvr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ikzdopxv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3vitehbwp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3wqqbjnie.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ggxwdolc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hfyidjcp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xryalgis.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3bfncbvwh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3desztvjr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3hnkenhie.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kqtxujow.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3befinxts.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3uvqcnnsv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3pvasslwu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3zrfnrtzm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3kwwzcpwb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qqicixsc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3hgjrsrzz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3untfypbl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xueqisxs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sqyvtibl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gngsmgwq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jpzhvtjd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3uxfkkwda.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3nhmxasrv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ypklgrxl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ksjbsuxq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3udnqyitd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3impqsykk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3xsscxjzo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3nezrjxni.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zwrbzjvj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3yjydzuth.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3efiblcmq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nsegxcnm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kpnkffhy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3djihyjan.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bdfrfmfm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kejeqprf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tvmflihg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3caytnhsg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3hwazltxu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vcoqdxdc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hexczkvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cuennvar.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3royvyylw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xbbtshww.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bitikzbi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3wtxwcyka.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ucyngmqc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cakictxl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lxnylvsk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3deuticbt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fvmxzkij.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qwuurxar.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vdfuvylw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3besmudpj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3htqhlkhx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3gbntcjyd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bqmcbzof.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3abgfhxex.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mofakayy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vxtaaqqb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lgxruyas.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zsaqrdfq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kivzmkfi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3qvbtfniy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xxcstqkq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sqkxarbt.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rtvbvufm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bmaniuhm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ljgemryx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3oivenyjn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xvldhmqk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3rgsvhlwu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3usrltpbw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3rtcopmrh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3vqzodbhx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kjkbzbqn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3oidertqf.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3rdiuxsyi.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mcbfyjdl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rsgrgejf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3gfmqpyci.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vleicivw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3advrfepp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hoxmfrea.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xjztmxjg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wqsmfcjv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ziloxdib.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xvxgptdm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ldqnfves.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3evgweqle.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3pycmefae.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kmlrnzxx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xmicyqri.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uhuztogh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rfggfknk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hxvocxlf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gocyuosh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tmrddpus.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ciprvxvt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3hokvhuld.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nbofrbik.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3jhcbkifx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ftnrgude.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3glcuugny.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3nqnibggn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3dthiolrj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3oxzlbwmr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3stxfugss.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3vtiahrag.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3gviaywpp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3trpmitcn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yzfzgylq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zcawgcvi.html


<!-- 参考信息 -->