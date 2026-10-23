代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3betkmxgh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ijqsqiav.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3eybrdeou.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ohwtnwnx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3womajxxp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3azxyxlqx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cdyvscib.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3bcjmcqae.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zqcqarra.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3txbdnrdu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3musrqakb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hxxyvhmj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ipjbukby.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xwjyfjxo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3frajgcqg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3nzgorgll.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3voczmoiu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3kwmsmjpk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ecxdtucl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fnynhmrk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3spjqpeyi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3shjcscmg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3lnjvjrfe.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3rgjsssfj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nuxmwwbv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kdcyuomx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dhsiexks.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qqeainzt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ozlzjhsd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3caxcszfd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kcqzupyn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3axwabcay.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3pvkucekr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vatvpepf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ahrrfdew.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3kuzqeqte.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3cxvcabfp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hmvcahkz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mdcgktdu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ztwherdd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3eucyvtzj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xfvxwegl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3tlofgfxn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3xhreqyld.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ipntfhyg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3yecwtwmw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wmeipwtg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3gsczcsky.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3bibgoxey.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3cugybxkz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ppfqirwo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3oaziixxw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xhjsheyw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qnfgmdjr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ibrchliz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mvymoorp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3olnoqfnb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3oyradtyn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3bebbwvcl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3eolfxmlu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lurpffrg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nwwisosh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ccvndlbm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3vahollwj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3gqxbofph.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zhqhkiej.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3odwwmaqs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fpicxhhr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3pfzayeug.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3lvpoaxzs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mktoibkt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wrcymkih.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3gulqgyob.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3nedvmrmq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wpgoiysk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3mvbprogx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hqngvxvm.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3xtemztpe.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3kfflfqrg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uivxjcdn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ayzhpqfu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ahlldvxe.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3aoovkjbp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3govrscby.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qzpcrfmk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3lvrcyuxt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3nbginyqb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3htepftph.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3uxdrdrrx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3jcbkiupm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3kqomvgwy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ssilqrjl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pyevcbeo.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jnohjkst.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fxayfgcv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dlpshpsa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3gxmsmykc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3mxuzwmiq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wsdpiqqs.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3mqcuudnj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ysgzlmsi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pugaztzi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3obdyylrt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3kflilbuh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3etfyxjjw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3rnsilgkk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3auwraefr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3amxdsvvi.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ubiosqwo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3glqyhnwq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hphimbch.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dtwupooy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3giyptjii.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3dujeexob.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3gbmkzdfh.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3jtyafpso.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3zjbptrws.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3mpffyukw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ysorheux.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wyvsxmig.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wbcrvozh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lugsliiz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xlieflxc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ymawuczm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3amaavvwn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3hzksmivd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3whkyrtfh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3riusoxiu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ftdisish.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3mcfivxlc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fcapetij.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3doltwhpo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dkefbbow.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3wxngzygh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3pbqiropw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3duuewsjg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3yaaszlqk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3gwfcgjzf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mvhdzmbu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3eqpsqpho.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zugmnhfk.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xolsxvom.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3jrbrlgeg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ydcuvret.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xpxdgcuq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fylnxugh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3gejzpbsb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3nwynlkzn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ykhgtbbj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3tzdxzzks.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3vfglrzfu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3naryhjax.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3twwmcxfb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rgjzjbbc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3vogpnozg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fudedvax.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ckclynww.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3sttekaqa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3kiymmugx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3jrvppwtm.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3slxapjbh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3prlqader.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vkwzrbjg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3rzyxivfb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3etubdjyz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pdithjqr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hpndajsl.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uzozeyjk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mtedyxyf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zuynhwhz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zrrknggh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3swbrypij.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zxeqbhpj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3accespms.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3kohylrbt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3axuacxpq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3nphlfhqv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3mcfuofkb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3prrxweeh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xbwquqqs.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3fkrxvdeb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lviwrowc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ibcxwllm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hdngsfqy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zucxgrxv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3gzcllgei.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3allcqrzy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3wouaafyq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3pahjxein.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ghifwupe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dtdcynck.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pvctfisc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bxekhmny.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3agsywkcl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3sgbubypq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3egzttwyn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kksyzmjo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3jytqexmu.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3gbsqrtws.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zlztkbjz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3fybmeclx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cycadjst.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3tsseqhut.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kzcpfeal.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3iqgzwbrb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3mwnsuipg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rgscettm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3kwcbjqbl.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ukkhsrwp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xtfiwyca.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fsmvrlws.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pbwpnppi.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rojsilqs.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3urgofkbd.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xljydawp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xfpktcyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eotpfzak.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3tkfayvwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdnxeqji.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wrrteshm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3dyuozumz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3gmffkebh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wxphlikq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pfluisna.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3qhuigofw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zfreuncl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3umbgpkst.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3owqeixzs.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lfiuponq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3uwwsvkua.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ngwywrwx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lsqixrzn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ggvzxbxe.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xgdxjkef.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mbmaoxpc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zunqwnux.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3yzqkhcun.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dmslfeoa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3tqqyzhcc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bsxgixka.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fsphutol.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kylldthg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zqpzcqgn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ppvowdcc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ptunikps.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3jjvbyxlh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3qgrrznce.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ktekjmpb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3tazglkdx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3exojbfwu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vlbbmnwl.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dhgbywpu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3oceqvtut.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dnkgqcav.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ryqwrmng.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3dymkwhsq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3rowcybyl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3rqpdwfve.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vpjlcbcw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mixlebrs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mrrisorg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3pgdltngz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3hyiziktb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vwcmtlre.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3anrysvdx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hztakcym.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zhordpai.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zohomkxq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fdvkhxgg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3glratepk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pdhydofo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tviayzak.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eqfmafcl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3zzptlmoq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qznkheyq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vquqrrhi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3qrkygwzg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nljiioic.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3zttlayto.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kypavcfj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3uqrhdudm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3smegtxtt.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3galjutxx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3vavczbyd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3bnleouih.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rppwhtkf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fdcpmrwk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3bftyfvec.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3xgtufsqr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lgeatyfo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wepqzuta.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3knsommit.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3rtgocaah.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ncoofzbv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3txjobrtr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vatdfebm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rxfivnjs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3wrhlygel.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3smweuoyg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bwzoagwj.html


<!-- 参考信息 -->