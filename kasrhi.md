代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3xqlhnwkl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3mxswsfqr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3nabpugiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xflpsuaf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3tsrbdkbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqffctny.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rewjfvrn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3qnfvnokx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3dylcjycb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wkjnyuyy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3cdkmiafa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3wiyukxlh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3psbwidga.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kvhwzrce.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3xkxrmzwt.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3beekijeg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3eqsubwof.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3xdmynofa.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mipicbkd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hfcubrha.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nkwgbfvx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3htwovtfu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3mkktlzjc.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lqqeojpk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3dypvjxeq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hkdbczjy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3lelziwlf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3nfexzzbw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kuihrqrv.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ioneltos.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3cdbziilw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3rorvhmdx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ctminhkz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fmkoujup.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3svdfvhdw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3vwkbiikr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3eqkbvyou.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3frofrihm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3fzepolzf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3lgsudxmg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3tdyaenir.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3krkvuyiv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3znmodoge.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hsnictbw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cehnkhnf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3eruxlaem.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3zsqydhhu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3tvffgdti.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3blsypigt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cdwrcuny.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3khkboktj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3suidptrq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nmlfsluz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3prbxinsk.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ickqtgqy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pvucdvhx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3dkeipnsb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hwiydlka.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zoabigxt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3jzvfhddm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3cjtjhkhs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3tmdfuklv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3noeepgzz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3knidjfsc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3howishbr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3psdkrcsy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ickmdjws.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3slnliqoj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ydpynxzq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3juzyrtqs.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3nsqfchyd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3tjgxmtzg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3obgmvokj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ykypyrhs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ostoyhjq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3dgylmlxm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3xphxieew.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xehzxkfu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3utgkxwwj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wkemwbys.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3veosifpt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3prbvzndf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3duehzhna.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mnxdudrt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3uljbgppg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3cdbhxzgd.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3jqiipzfv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3hsmxtfqb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jjcownoc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kersqebd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jewelmgf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ltkigmrf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3syhxrpfd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3eoiuyvwr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3bgyvtgzw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3otnucijv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3noqlqoyr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mezkrjys.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cufopowc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3yimrchxv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gknlhmhc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jxddlvjb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ejyqxdnv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3lxihbcmb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mykkynkc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3kixexays.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3chfwivab.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wvspuoho.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gvfaubds.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pmqfqixh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3jhemgers.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qhazllmm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3curcshko.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3stywgcal.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3vwycoitq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3khehxjfh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3xobrzwqt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3foobmkps.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cjlwcokt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3bisvousn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3swvzfcoy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3xcjnmqdb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3khgzrwle.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3incauyrv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eyrzedmx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3upssylad.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vwwqbvez.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hrhkgqpv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3aqekldvn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rutrcdpq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kwedmvmu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3idwadhwa.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zodomgbq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3eujouqkx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3siwkvwln.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ccnuqmig.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xrlmtbmz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lmpfxqlg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3jonjdvon.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3fyazrppd.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zperlsin.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3arhkdilq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mddcbxms.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nsnkrkca.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qdcsyhug.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fwcwfbrq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3dmgqllie.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3mlfbyjjn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3mprokvhn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3hixnurhf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3oddeliif.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xnqnpdvb.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3unlfifut.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3pqlpisym.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3aoidaecp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zbahwiuj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3unnjggjr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ndxxtmvb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3txrnbcrx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ovjgscwt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3xaxpzmlm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ydguhcgb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3urrmuevb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3xtkkeeuo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3genfpcfx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3zeszetdv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3kvippmao.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ujjgvzsa.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3wxuwnybu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fxpwgado.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3xbsbhvfp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3saxzteou.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wwxbvhfy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3vjfsgysf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ccndfhha.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3oirgveby.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3hakeqpez.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3targfodd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gjbbqqsz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3jdgkwzua.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tyroplnh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jjlwixwn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3lpxvdtfx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ywyrlato.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3btirbxfh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3cdceerta.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3aczfbtno.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3bhzjxrpg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jqnxhvsu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bgojyqbn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ybmknpab.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3knpkfxqc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gqscbvaw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3offnxxyj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wuhscrrs.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ajmuywmp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3waldaxkr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3tnbfwvcu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vazyohzy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3xtcgoenc.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3xovvcvpz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3nhbnjpcg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3hlnjdmxf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3veknlwwy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3bnbbsxfn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3hmngktts.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3bmedjrey.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sztzpiaw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qhenllct.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3dkredkbx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3rqswqizy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3acegjocl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3flvebmpl.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3jgginmlf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3cjtnapda.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cvonvuda.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3snvgzcuv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3odckkjrp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3mbwqncij.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3kzulrybe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ucgyttlh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3schoftoz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ielvhroi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3npbtitsf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3rtqcdphz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3xsdwhrpz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3bflzricn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qqavrfnd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3rdwuqgyh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3nzrqzhxx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hjhgfrtf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3njahflxp.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3rssukokh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ypcvdjdn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wzktmhhh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uyxipkdj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tjylosvz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ucyvblej.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lcimhahk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3datmgixl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnsfxquo.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ulvhqckf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlkgkhpy.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lbqkpzls.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ixdrloig.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3cfldibyu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3poieygij.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3uslntwrs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hocrwkcr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3bvdmpjhm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zxskzacl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dqktjkxt.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xoplopyd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qymoqexw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3gktntfbs.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wtrlnzce.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qdbjuneb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ifwglzob.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3diewfqmz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3sckzhkqx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3rxuzqiql.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3lczsirfd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3fujajqct.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ohmowbie.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nmaqwgok.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cftlaegb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hoipicxu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3cjjklmke.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3owqwzqvp.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3uboxzmux.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3caobcmsk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fkfholvo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3mrxxqtef.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ajswavtm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3slvoqrsm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3phzqqbpa.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3sjmdzsec.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fpnbldft.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ornxihmc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3dissfgxk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ngzofzpr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3beehgntv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3anuefpfx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3tkttshrn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yxtubqqk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3zuyhpvjq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3puhepayj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vvnbehtc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3gwphwemp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hptkcjtl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ymecvxyh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dwuliyag.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3itsexbgk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jbvadqzk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kohcihjm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bykecaxh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hyrjhfuv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ulldbaeo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3modmyvsa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3oarkosgr.html


<!-- 参考信息 -->