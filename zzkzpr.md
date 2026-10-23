代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3njzjkrau.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wwkekahh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3kmwdpzum.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ldzeopul.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3brljhsoz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3cqwsxjok.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qimsqxxs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bilkyrcp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3qjegianz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mhrhopnr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3lwegwnkt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xdxyjgmb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fmatclwh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3bwkolhdh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3dyaldijk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nblpghsf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ocwknxvw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yttnrkur.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3nxxtkhzx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ibhdqohb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3liyrarog.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dhudvylk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3obmltrds.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lmxmyxij.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3txcducze.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zpbqpusf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gxurejkj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3sigtypov.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3wfrjaejl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dxpmvals.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qonezsnb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3phqrvedg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3fpztqwue.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3xzynnzxi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3eakngmqb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dqtvanzj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vxabcgso.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gwgnkhgj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3kmyzehxp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3yffcoyzr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uutzhlxf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3qucpwzvz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3jyaxvjoy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3gxmyibnt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3avdwiouv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3miqfpiss.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aigjqjgi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3gzxwooev.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3fuftkwpj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cbewohcm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ozesahys.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gdsbgkyj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3cliqwstu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3neuzmkzo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3hixmwdix.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ralfzhnz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3euwigumg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rnipvree.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3bifwfzsz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3nzhdueco.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kdohqlyp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uhfmnlle.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3baodrfkc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wsrlkvxw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3xgfmpqye.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3fiyqyarm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3onmujnje.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ftxvnufi.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3vqtlydbk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3xptqvcbz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iuotmlqc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qjrnvled.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ugmrgqgy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3daowphuz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3orckpslc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sdzvjndi.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jhwbawhh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3czcrqipn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3meeeacdj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3psvdsdrj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tdcddjvt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fktnxeim.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3hkzvfwqv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3icsdbxag.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3kjsbphqk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3tfvluvdk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3fbelkrzc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3nktciipu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3twyovqtv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zakviuui.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cfwiewhs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3trjgdiay.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3agtdpkvd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ejmjvzrd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cojerxrc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3qnoiovbi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3lvadehpb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bmpgnzgc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3caxcnjcj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ykekqzid.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3wpregubx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3iqdkkzxt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oxovrwdk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bfuamanj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3devedvlr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3twvdaqhj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ufrtbdne.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xqdnliod.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hftrkrvk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ymjqsvud.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3clfgvrzv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3kpjirndl.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3xyrnuove.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3nadvfgik.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dkuiluhg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kelwcuau.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zzjidwsr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kpndkpuy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3xzgximfr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ewfmoegv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3adkmfnmh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3rjwgardj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rwzxnyed.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ogxnorqq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3liuycove.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cewfdaww.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3kcrkywjw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3vvftqblv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ebvwhciv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ndgehyzj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3omgykosu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3sctjdhwp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3rotprsfb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3tlscotwp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3bwjisghj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3hakdrond.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hdzcghfm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3fwoznyma.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3mkdkmaap.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cqmjfnfd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3sibxfqyx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3obyerykr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3sluxlzwl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3tiivalag.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3sejkbmny.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3wamtdbtq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3jdryptxm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ulyabtis.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ngnvumkv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dkrbcbmy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3rebedecg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3lizhdnds.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kuoutocj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zudgwzid.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3hnuulswv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3pzrafuge.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3hrtagnxq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3vnkjthnk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vpsitebk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3bctykulm.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3edbxsxws.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qqdqrcgu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mgfhehwo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3azqljgzi.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hzffaovl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xggzyerc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xuwbopld.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3nyvrzbfb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3pvhijxnb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3bzybshil.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tlnqtqjj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ezpoxwuh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ycphnwbv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3jqoocnck.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3npmtoofz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qxsdzufz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3mmfcvycg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3gklgzhzm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3itatanak.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jiezbjaq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vpdmwvqj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3authvlql.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ujaxrabt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3axjilbcq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3sypndqkk.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3bwhkyouw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3qsxmewby.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3eadyjakl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kyalojiq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3otgvrswm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3cyuoeqhc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3xkauyorm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3otafjjbx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3wxrlygww.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3kwfyeijs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3bevdsyuy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ylbgjgck.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3iesemdbe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vmobzfxh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vlguvmny.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3nypowlqc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3netftizl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rmmffuhw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mpyozuxj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3egjwmhli.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rdisiohx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3goptdtyd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ollosdqf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rzdvtrhd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zibuzhqk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3emswqtfp.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3htebsxiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azuefesz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3fvjyczkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afruznyh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ekbdjctm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ariglzcd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3mfpjwxan.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qbyvrsye.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ihxdiafu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3rxxrxfkz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3xbyzgwnu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3yrtxwpog.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iivwascz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3wbkiygka.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vdtgofhx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3snebaaht.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ldxddmtm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xeglsklg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ljqalvnu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zhjtkuyy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3sdysktgl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3rfzqyrco.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jlnxtvos.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3chsoveta.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kpfvtgvp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fervdvgd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3greiubur.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vbfyapaa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xceracit.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3eygmpoyz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3klpvjqdd.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3fkontfil.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hoiijmtx.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3gftuebrl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ujvebkdo.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dhrzkbfj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jgkjxqdn.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3gkmlodhn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hwgbvdzj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gztobxzb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3unvbryga.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bupoxbam.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3jxjtflom.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bxhmqmkp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bjkjfouj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3avsfkqzq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3kitujeem.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3thptrswy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zuzoxded.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3fwgutatm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kqnzigvu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3agwhxllj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nzhwaigr.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yuqffukj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3frylgapd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ksfxxztw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nbjcxffj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sodrhihk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wvjutfra.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3keejwevx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bwwaghwp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3uhlqkzyw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3nchviqdh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3uemhdoco.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uupdgabe.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3qyyzdhia.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3jhzqlddj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3bxgrwhue.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3wldnwjfc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3npjxaaja.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3krwdfduv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xylaedpq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kxfenklk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3iehhgcna.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qttyqfzh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3bcsbzlms.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ygtgpfxe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3cezdsitt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jipilzfi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dlhpzszb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jebzyxpc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lwparvai.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3gtvzhiym.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gvztaofm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pnqknpaz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3evslksui.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pdmbjmks.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xurtapql.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3syuwidkp.html


<!-- 参考信息 -->