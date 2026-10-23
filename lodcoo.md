代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3lfbabprw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ttzlkgyu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pckluonq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3otmyllrd.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ozvrdzba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phrysjwb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3uyfdgjsy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3gaggmhyd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tbgvcigk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tvpzcwcn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3biijwodw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3veanrikx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3lufohluw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3pattyjbe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3pufxyvve.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rafmqhxd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3lxpjqoza.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3gukzczsq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3cohdgwpn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zcoqtmux.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3cxonqjnr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xfxlqxmh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ydpckbqv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bbmfhmbq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3qesvnxrl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qukrbrbe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3azjgkxlk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3pwzttals.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kvcnvzxx.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zqrvhjln.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3zxclejye.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3hmmqgeas.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kdxksyvc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3bjaztnff.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ijrdeaax.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3dzehscsm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3piekauva.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cyzycmoj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3beagwjqh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3dupqrvry.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3mpdaxrqp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3hafsgiky.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3kjddeunk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fxlmxsfd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ouphsrqy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qnmsnwvl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3lnedwkak.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3cbzhbbch.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3eaqmybyi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wmlqnamr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3emwwlqhk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3icsabfqh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uovrxmlw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xfwrawtg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3lmnjikxy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gutxlrzc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3nkhjbuqj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3volqkadz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dluxruyt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3fdzrmjwc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3anidxfbf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3fssaqlgp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3izcbancb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yraapuem.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3amszpwnd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pufxlkjp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3xtwpbvuc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vapkcxeb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3agzieyks.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3laovzefs.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3bvaoecei.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3czjzarou.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3jpgnzczc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3zghqivlu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mgzrczwi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3laezgonx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3somwegsb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jadkivzr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qrjkclvc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ailwjwci.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ojcjqtqz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3wadcgldz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3mhkupcdm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3zryziqdf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hncrmbbc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3agqaylhz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3aannlqau.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3jmmgwokq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3zwwxrmuo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3htjdnhtm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tntaygqp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ztgnqehq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qtkyzgef.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3hetnktle.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3rdwzvfzb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3rmjswzlk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3hlbgdiog.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3kspvqlrv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mjloxmml.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3bspenmxn.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yrswhcar.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ygsabzvx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ltxctytc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3kaanhlzd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3bkifrhtr.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ovtoxtkd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3zdebebfm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3itsouxhb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3piiimvwx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3chrfsepk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3pujmhdip.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ykcbghwg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3grhajocc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3iktjwwqq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3giytafbh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ooqmepuv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3krhebzam.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cheivowt.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ehjaaulx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3furqfijp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3slxttndk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ldasowqd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rtuchmyg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3cwkqprai.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3nywqjhaj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rwpahbwf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mjwoppcq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xzecjild.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gtsafqcv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jjjnmhit.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qtjhjcvn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bmaxexlb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ccmpmkbi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jkjundav.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pfjoirug.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3plrxjmdd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zqadibrn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3rmhfgtaa.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3bmumwphx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3vtgiogwu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3phijnrdg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3zrfmhgxp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ykbtzglv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hioakwzx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xvzwgmjx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gvmpwsjm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3hasetnpg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3tjxwvcns.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ndjwcmvw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3fpxtmnvo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hrayqvgb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dnjuskoj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nrgijdcy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3uacnkfqe.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mctgammc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fcbwyrbc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ikhjuwjo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3manuspru.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3apetayyr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3mctxbiqd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3dxalltge.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ihtytayh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3hsdlweum.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3woubwwvo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3rudsbzbd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3jzxdozfh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3iixkuceq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hepuuujw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3bsbkukyz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tnnksovy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3sqdappjp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3bemchivl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qyefwmfb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3htzwjvwa.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3qzeauvcx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ecmugnze.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3hmzvqnxc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3pqfbrjxk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3xebadhqn.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ylppgwbp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rhfnjekt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nhdzrlnd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3jnbqhjla.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3iqjfmgtp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ietavhpc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3jacnqzht.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3vpunovun.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3buhnxsuw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3zthcjwdj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jaoarvsk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3khnivrnq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kaobzjpk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aesigmcc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uvtlsard.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zymowwip.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3uvdsxzdc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3btkbjlyb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3pqznyveu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oyktahxv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3pcxuukxn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3atpiuorr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3asovvqvi.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rbxhvfzv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3hquqinbf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3gvvgoxqp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3knzjqsxu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ghwrmxmk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hykqvfjt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mviochcn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3asgboqch.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mfaesmrw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3emsvcnfn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3xedgmgfi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3tekhbfat.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3rhbwotyf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rtectacr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3didcztop.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lqqhditm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3dxzdjgjb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3srtkzdgp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3djohhcrj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3kzvzbguj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qntpbnge.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3mbikvfkg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ywexpntj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3lftovqph.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3tpcnjgen.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jwnhjxjc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3axlwilpd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sldbvgtw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lscatuhn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ixzmnjmt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pekdexfx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lfjbvtkf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ubflzyis.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lhqmjzdf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dqwnlalr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nwzbkzbz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ejmlsjvq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3inzjimob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dtmjmqsc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3uklffqlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zvooyqok.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3adywdngv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ymlpbzey.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ttiwypml.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3exfsqvta.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dplxrwtt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3cpqqexas.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3gouupbtg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3cognphpb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yqzaheev.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3cwhxfmcj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3recyymzt.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3daofdszd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kgxsryta.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3asldesok.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wkjwfagd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ozodhwpw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fmhmxnnn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fnnpktbv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nxpqymfr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3qmnojnkp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3limivzyf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vyshbuxu.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nbjsbzgu.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ejsvahyp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wsqmoghd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3hgbnnlxw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xkeezxzi.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3slbzkkkq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vhanblpq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3lpupeqyo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vytuwcel.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3skgbapod.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ixchitka.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3rucxrrjw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3glpwajew.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kmwoblct.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3gowtojzv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qpvpknqg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3nkwgmunm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kidnsaqu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nzeanssj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dvemjjwc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3jkeuchyo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tdgbinsc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cpajutso.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3fmijdavq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ndoyncse.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bzowdhoj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lmucuqur.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3akenmwps.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ldhvlaho.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qgbhhfoy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zykvrgjn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kcjyazwk.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3nekidwvu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3gbumqksu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wcdlrikv.html


<!-- 参考信息 -->