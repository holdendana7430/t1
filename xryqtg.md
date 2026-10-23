代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3eivjwgfg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rtlsywxm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3kyercamr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ujvqbtmr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3oxucpemx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vfmuxxox.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3niulbtid.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3sxiujhlx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3oclmnytb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3nyjtyapm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3slgvaimy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ozaasqzb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3qlnbaauv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lgumhhcg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3rucstrmp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ycgfyniu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3pqgklhpz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3evziqrmu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ddpzoyhy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3qyynqnyx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nkipuinu.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tmhzzsox.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3oferovce.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ihbcewhs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rxfvccqq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3chkwbpmu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fyjfainj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3lzbnqtee.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ghezljdx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ggpgrhxn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ymhcpzmb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3qonsadup.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sfacczky.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3hpiaeioq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3dsjyayyv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3stjkhkmo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cktsgolb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fioksgwd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3qwylgtps.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3jnqbiihf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bivdvfhq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3czbiuirn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3evmdyqsl.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3uhkxcgwv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ktukedsy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ojlubuqv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3yjgvbvqw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kdkxiwoi.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3udagfpwt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dkxzqoiv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3attuemec.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ensmdziq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3gdcggphu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3lcvntnas.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rlnnxpwv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3morghzuf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bavxgjgr.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cpilwaxo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3lrtagkyq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3xsecsugz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zduhyfpd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3gvkufqub.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3igworrsx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3zzpqxqbz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3khrxqyjv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ighlwimt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rubjljol.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3veilshlp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3zphxccer.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3csytrivr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3btuewxva.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ivgarzqn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3mxpvvtwt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3jabfccmh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wrafpnem.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3cazppmmo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kqzmwoys.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nccyjqzo.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3risvvbio.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3hworetss.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mnhjgvrq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mlolmsqx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3wmujsqkc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3srpfifqf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3seydrfcx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rgfwnonc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3aelmwebp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3gdvgtwbs.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3rlakaahi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3wnunudcp.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3dsgwpgrf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3hxaofclk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wltdyugz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3hlvvqdkk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3iwkchvoy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3zjoibtka.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3zfbvbebn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ftcttqso.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jgomftoj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vauepiks.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fdlmrrcq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3uvqxehcc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3nqlgeyle.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wmuznlsv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3kuyjcvny.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3lbksrfqz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3taqptmvm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3keznpbtz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wvknnthf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3yzfnkroq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ocdnkext.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ybxotkai.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3qzqgshnr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3hdmevdzi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ubnurfoq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3zpermvpr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3dmixblyu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pzooigwl.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pyqrqpex.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tzaqfjrc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jzhnqqel.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3gruxpkxq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bfutadid.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3eblrqwtj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3swvyqzmr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wnszulhq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3garfbsym.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3paxpoezi.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dcvuphkv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3rpyiosyj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3fjdwddvo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3abnyrfln.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3lbdlzjdp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3imvlyneh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pylvhseh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nearoiok.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dmoqmyur.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yttfgbxd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3yyoujrnf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3yjnyqahn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tjnmawgw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3qydnbign.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3yznxiybm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jpinagtb.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3yuzjdfgw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3wjsabffq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3womfpojf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iluwksue.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iawtacot.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3idyiskvq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3hepehcvq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3mleyyrht.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3mqulqxab.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ixvtstvq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ahwundps.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ngosmrdg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3hlzdtvgk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3yknxgqxa.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3gswfcste.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qzhhzyqa.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3jmwjjuqd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3vsxdlryu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3fyegfero.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rsyzvqjf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nbrcszjw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ehkbrvde.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3qcxlcfja.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3dxcdwxyi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3iqubzmxh.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3yepunosm.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3cypnyxwo.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ptwvfvzd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3otuagizz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3djzbqbhi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ajnaesjo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3oonbepoo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3hnytgaka.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3uqvmjovi.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3jugoewvk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kxcutqbd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3eaayliou.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mgfdtztz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mzefkndi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uxqmdckc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ymmvnxyr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uysjnihn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zofopdsp.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3kqtmldlf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3xgdhhbfk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3wbrxbmnd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3pynmvolx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3pzselgtb.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3mkxzikdi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ztgadwpu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ifwphlfv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nbukjavp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3rzlqdtrh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3mcthkvbk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ljonbmbp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dbjsqokh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hogbpgho.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3yxolxzip.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3prriyhja.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3pwjphhom.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3huyrfwms.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3kxobesms.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tdzujryi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3jknsbbsy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3wdwqrwzr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iumjgoup.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ktoqzilx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3iavhmguj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3kwrxqgiq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3yrpzxwlk.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3nqrchkhk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3poipftlq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3qvcjuhuh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kgsxbkwj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3oyhccdod.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cpzltzrl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ugxujyzx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3hzuvmoxj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ztjbhxdy.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3dwtxyajx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xfzmgqwo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qdyffsdc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rtcjxnwt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lmbessbp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qbctofwi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ijntaiam.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rzfsowfp.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3xwbsogsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umozzvnm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3rdcjqzsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbvhtqws.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3loeusywe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3wnacxnmv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pjikzwht.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ciyddkvp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3prrtcdbh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3nbfmaxwr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ujysqmvr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3tgfuxzmt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iuiblyam.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oubyarvq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vzsfxcky.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cdsppsmi.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tivrkuvy.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zmmzzynk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rrbgecjc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3tpqaawew.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3bbqsgedf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3vwonrrda.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3myscdzhi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3zhwdvwgq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wzuszysw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uzbwfswp.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3axmzopot.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iaubtdcu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3oklqmpmz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3wlxbdkwv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eugktnyy.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3iyoxplkv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3pgaogvij.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3xwdnczhm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3wxwpeupr.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3btlfcqud.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xmauovjb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3wiostomx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zwwgmnfv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xofvqkwe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ficulnyb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3wsakmbjm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3hctphsuc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hoxiqhfc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ikvqfeod.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cacwsojv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3lehpmpzg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dljqsvci.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xcxuujfo.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3hwsotqzh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kjvviiql.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3mxqgndoo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jdbssuwd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3djwzqoxp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xcdrkras.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ymiibime.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hjdomvij.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3flezyums.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3mhfmxfka.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3huasxwab.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uwatmjge.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3fozdegzv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jynjkftq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3vsobskfb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pufrhmfp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3rwexpqvd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3yfzphsnr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xxfkxbvj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3jajiaxdy.html


<!-- 参考信息 -->