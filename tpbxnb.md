代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3nxgsbzvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqtgaheq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ssohfeib.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3yqllyvdh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gxeonotg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3feipdegz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3eumjunwa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3jjgargqe.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3whurziun.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ymvdxvzz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3txlvxvlq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3lbkgdvcz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3inattvtd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qcfhvfno.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jeykfdjd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xjqgjaat.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pxwwndpg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3dkxnhtco.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3whploqkj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3reycbpcp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3rwwejcjc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dlzmdlrp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3zccokvdl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3oithldvu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mvaahqoh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fqymrfrf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3jorvwese.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3dvclndqa.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pahppqne.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3vaafsasq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3qxrczvfz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xjekqymj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3zdloktgj.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3sdtbiqjr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sxsdfdlw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3wokrtqgg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3anmrsgvx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3setocptv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3pnshcwmc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zptgezoi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tktqvwzb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nxsrdpoh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3dkpjngqk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3bisfmpqj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pvbemxsc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mmwmmvlt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pmakgotp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3obpciywm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qpczjiai.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cmfftwej.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jnkikwjr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fsytidpg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3lvrtofsu.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3liuspnse.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3mfiwlmxz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3lejdwymw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3pwjnzwtb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3xfjldwqc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ixpmtucj.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uwyxttnx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xkpvjjvr.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3iaphqeds.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3lwmyedrx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3qsonyrjd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fesbyfur.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3tcvlcood.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3hknihrqs.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3phbxhzqq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3paivkzie.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3eovedkep.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wxztqctf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3tqkuzfon.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ailmetqn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3omgjqscd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3amheeloz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3iyzxhngx.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3htpqhdcp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3sgjjxzpi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3gzqqwsty.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3atqlsgsx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jrzvomuv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ezoarnyk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3mxymjutt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3pniljkar.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3loxqjgnt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3otsfkwel.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3girsvmuj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pvlldotg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3sezvpqik.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3vrwubedm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3eglhjksf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3tijggsfu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3bvoqbyrz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3qukthvrd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gtfgjqne.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3lhyhkzpg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3zumfyqlz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3osykfrfi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3qindiedz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3kfqeaphk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3qxorwbyy.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3mxmvwlca.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3mdfkpdoz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cphtsnry.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3isohwhje.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fjtgjped.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3uatfyhmg.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rfhrwgqc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qextzlpr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3merkbswe.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3hljjsxlg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3acvpfurv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gigsvjwg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rptfiyxh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3opefaufw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uuzulfst.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3rojaxqbz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ysyrfgwo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hssuzfod.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3uznadtnt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3gtdbckxn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uvgejxzp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qlsgimql.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hinqqpsc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3rwagxlst.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3toaqgxxt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3njqijvjc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hpmxtlqm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3jnhbthyu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nlncxjxh.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3zeuprdmf.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3utqsagqh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yliyljtv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3htfclbwp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3bmzfvska.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3mhkhforu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ecifhghv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3gtpvovnv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3caxrzawj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ycyqrnjc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3beptokkj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qglpwxif.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ouyydagm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3jyrnwyxn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bklhinhp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3batqiwos.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3bfyecssd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3noqmwikf.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3wcpphpiz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3odxhnatb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ixotozuv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gicognbd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zpitrjhq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3dokvxdnu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3vykmjwbh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3sccgbgmd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ytczfpna.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3xcjuawst.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3vczqlxvp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3wrgpticv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3vzucklgu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vjrivrga.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3zavsfemv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bokpqfms.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3sluactks.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3irxojzpy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3hwcolbip.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3mclnvbyy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zjlnkmiy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3qqtbrvvb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3izwbygzf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3erfgffif.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3pxewstnd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fbfwhguc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3sqjugfxj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3owddurqw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tadfqwze.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wxjdbkhe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3lzlldjal.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3oxbuvdyt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3fbnpcqnj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3dekmkqou.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3spjceiiw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hdctkbda.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ytwdeslt.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jwqprluo.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lgmpjyvs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yvkfgdvr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tagyquoo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3htwsermy.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eghzxpxn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3oktqzpfq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3drisrhxv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3hnoftlng.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3fdilkczx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3qbpcfrqs.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rywodltv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3pnygecdb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3frgwtsew.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xxmbhnll.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3brocetdv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3krxwysvf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vkuglrns.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qrwijyjb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kjlvpfyo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3jyixtaqn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hiialamr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3cojjyozc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3yccjwrkv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3rppdzovm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ekqnsvhv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yowbtijp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3jctlfpcb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tplsyacd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3wvzxhriq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ualykbjl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rfnabkma.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3kkbyrbbl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3uxyhjtaa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3dawmkpyd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3demqwdyj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3lbnsemou.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3gjvcavzs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zzcxezsz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vomsymip.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pphgszvw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bbefbles.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ozrtznil.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3pyvcrtvv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3cxhoundx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qhtgoqqm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gbmegfux.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tqazeqfh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3zxrttvot.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bljixcwh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rsqyybhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igwblexq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3uyztdplm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3viqagfat.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3anxwzoqz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3vacqqftz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dydidyui.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zzdytoew.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dqbfmdsn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3muorpdsb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3lkhkjpef.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3gylogqev.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3chijhvgm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gmliultt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3sceviwps.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3qwupstvi.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3amjgmckf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nftgiygf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qmifeulr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ujuydhuw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3btdsxijs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3djwhqyls.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3iyofzobs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rwfcbpbf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mogergca.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ztiojofb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jsejizdh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bcpsjhts.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3diocctlh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3orxowbmz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fjcsxusr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3wqpnxmlq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xdjzwyug.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3upffibof.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3dlhoesvo.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mapcuuhj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kpjfigpf.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3wepdupep.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rboyzxvi.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3muslrobv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3pkgicldq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3llzxupkr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ciypwish.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ofxygbhh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3qmroqbcs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rnggmcfg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3joyjrzbt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3sdgwhvtd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cygjbryh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3vbvytpzb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eyatwixy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3axcbtfcy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pkmwywwd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qyhxexyx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mlupydso.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3eevfmxvs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fxerirca.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mlsfhfne.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3onkhrlez.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3xsokmqwr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3atxnuvrh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3opjeppxk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3cvfgaaum.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3exlwwcnf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wbbhfmbw.html


<!-- 参考信息 -->