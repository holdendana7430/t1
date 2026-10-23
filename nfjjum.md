代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3olgjajak.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3izvvgsjr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3azppeopz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3vwclwxgg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3obmafcsu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3clvrxeet.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rezsmakx.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3cdtoymcc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3imlbrbfj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3stpdwvux.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dwqrrtae.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3pcmabzsr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3embpvxxs.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3jvlzfcay.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ysasksqi.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fwygtrtf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3tvkareci.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ucqjxjwg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3jkegjfcv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3nniwzprr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3belozzdu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lvlgqkmq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3agxqsizo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3asqkeszp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nhesvwdr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3czcmtbfo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3odghjmny.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ehwxhmzy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3sjcntdjp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wuchcdui.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3bgnkrivz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3otqrhefp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3hosibnpx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dbbghbkh.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3bumtxele.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cvjurwhh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rimioduq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wrqxuwhs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3omjufrwk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3qrzfvypl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xnbsbiuj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3znrrmzux.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ncrwcflc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pyneuyfq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3glceaunm.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3fioshuml.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dlqwlnrw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xxxfcfqt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ofsmpxfk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gpgstjao.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3rzfzjerq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3kejmixyt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3hfttanoh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3omffufst.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3cyjfxker.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xfuiqedl.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fmfnpqaf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kuxevxet.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3egzbnwpq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bphvbdgf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3znwwcmxe.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3fhubzzqd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zggsppkk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3edhtslee.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3kaiwrlgy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3clmwkryn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kaoriiex.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3bxtvcqgz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3hnstboea.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xgljqpxi.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3xvhkrohs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gqpbbjcm.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mordkhym.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3dtwcuueo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3uocabodr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3cehgwayy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iktyysik.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3thxbqiwj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3lzgspxtg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3uwzymwvk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ymrtxblm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3estrzggo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3znkbhucu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qknzkzjd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3jjosoxqi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3kqkxcwis.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3aoampczb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3qewqlbfl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3bepbrvlf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3hcrjbpvl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3byiptlbh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3pdyqxssi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3zkvykzxx.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3rppnayjf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kdjankiy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3qpqvltui.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gcylqdez.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3taehwbdj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fibjfjyw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3qguztqbw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sggucrzo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ywiiucix.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3iiyupkfo.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sjfelxgs.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3grqzpklb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vzxmesds.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ruypsqim.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3llwvfefm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3kmkzekgo.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3czjjwzla.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cvurgfsm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xdmnujsd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3zyvnaync.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3kyvzaxac.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sqruevjv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3kvxytyrf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3lywvdfgh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fquwymtc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bwvjknjm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3scodcnsn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3nxqtdnxr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3yfxwntgc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dqotzune.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rrwqptwj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3qfgysmdu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3caljitgt.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3qksazrcd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3aofcmfoy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hqcbwyon.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3agyalgda.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3lsdrbmyx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ydnquzfk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wukjplzd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3rizpfrzs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ppqspttw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zadnkggj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fqwmogjo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xooaooue.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3golqglrz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3daijgmyh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3xcodszcx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3lvnuzdnv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3sfplsdwj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qqtpbyrg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3btuofyhx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ylcnkelt.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xwqongex.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3wjdgmmqs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zexzdlrf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3nuosizoh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3sduaooni.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3pdykxrna.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3akoojonn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3isujnday.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3zrddlhyq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3idxsxbum.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3trazlfdz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3yipkzzgn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3itzkvwkv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kfhdqfft.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ovjrwkhi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3uikdtbvi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ywjbmsgn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3lezntqez.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zhxzfnht.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3hqsvrwlm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3fbapqyfv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3zeolcqdc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3icyhqxtz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gkjwlmdm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cdflvjum.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rcdgvhvu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3aiqwmibu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vjpwzrzl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3hhjuoxho.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3cdupqtwe.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3riikiuhd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3dytraojn.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3lmjutvgp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rjlugwfn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dpeshbbs.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qiwzjxxg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3blcezaxx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tothbbck.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rpoyeonb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oysrqpol.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xzzwcdyb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3njgyvkbo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3txxxovpw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xnanseat.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rhizxdaj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qkspqtmv.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3zcqhaqvf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qnfdzmqq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ehtjagpd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3qbviopnx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3cgduqoyf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3hoiczwsf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3pkcqrfwm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ldytvqrf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3gqafpppe.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3nqimswyg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3azjzdrsd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3smtwehid.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3cyfypran.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3nwjkmmzr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3pwdtzelw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3fidjlsod.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3qoyjzotr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nvstesyx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3aqirwcpm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3urtjtyft.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rqiypwfe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3nlbsfora.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3manlyxaq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3uazizyvc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3nwadpett.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3lpcllbfp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3fsjncadh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptnxufvq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3yjebbrzx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vzmozlxu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wimewpjp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xjqdchtc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nalwtgcv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gqkwhmkp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3iheyzzxv.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ibymvspj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3umrplxih.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qechomdo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3opmbclvf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3pysbqwis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbgbymet.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3asszcwfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xsjuinhv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wxcsgcml.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3jzwufjxp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3drohtpee.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mletvmmq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tjgzkuvm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3cakjamkm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3mkogibde.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3yznqxwot.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3byypqnrc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xbttsjqa.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3uuntvqbn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fiuesbsp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ckiqmtie.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jroonixe.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3afaujwxs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ghacmixs.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gqiylsej.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3duwsfuya.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zkeykcft.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3muytnwxv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pqydkrbx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nxvycglb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lbbvinoc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3udvyosox.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wwzpwulr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3elarfutv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tujwkntv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3cihlnmvq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xstoyyzb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3jssdhzaw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3nafjlwmt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bpftreje.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qhdsbein.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3frtnsmmg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lrclwffg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3onjnnbea.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3wireezrd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dqulrcry.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3tijuckyv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gesrvllr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wuefsgoy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3skzzstxd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3brhrdxwq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3qymyqxpf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gueuacnq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3lassbqmj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ryxgahqs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ackhgpvy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zwrrnlcu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zhfgshmg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3prljjbcz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3atzjytpi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wvkirtnw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rrzxjnjs.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mglxqooa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3gahlfudv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3odmiyqxv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3thyzolok.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sccsxgxs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qnlnzokg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3yijgtwjk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3cyedfshx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3uubekuro.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3yvlmumqb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3obbyywaj.html


<!-- 参考信息 -->