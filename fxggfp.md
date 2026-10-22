代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2dkeswuko.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rcsbujmt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ntcqniii.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2edddcbqv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2iimygngj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2aobvhpyi.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mvmvdhwx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mcroicdz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vguuffra.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vefgakdf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2uczizoju.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2edtrsicg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2cckezopn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ajyfhncg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2nuxbulpb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2wmzmtzuw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zabmkbhz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fdqvikof.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2sjimlmeu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2wxllztow.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zocndgea.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2norjnpee.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2qpepbqsg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gtdecevi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2yjmovhak.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mnzdrksg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dvcykmxb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2xasxqcup.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2suhhfagu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2mqhvkemd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wsiqtsrd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vuvjecif.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gpyecwfl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2iojddjst.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zhtbsczu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2hklraqww.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tbiphkyv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ipaendey.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nkdzhutg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tghsqwdy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bznrbifg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2afxfecse.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hfhubnqa.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zzvdshnt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2alyizini.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pttvdhjc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2omneaazr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2wordgnab.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2dbwllgun.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ghiiybkk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dwoeyxik.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wwpmwrqn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pkwxppou.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2awbvulmd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2uojmanhu.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2trgzgzmo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xlokxyzo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2yionkpij.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zkqrletf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2phklqzei.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2gvzpsagr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ukbirzyn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yibmeech.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2cvthfprb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2cntemtyv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2svycqcvk.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2pksnweks.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2iytisxqv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2brtamtln.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2yzeiucrb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2fqfruqri.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2rwzbltko.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yimlfsvm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fecgqszw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ohxfhuyh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nrjmlkjh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2dblmyhyn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2svljdtml.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fxuylkbi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vwpibedt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qmdsvdhw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2xblprmuq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2xrkrwniw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2xwhizvvw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2odwgqbnm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ywllptxj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2harzovzi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2zsyohizw.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2biyfkzgd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2twptexje.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2rpfigdgh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2xldczetd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2wofxlqgw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2gtcairfh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2oylzhyuu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2seuylqsz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2uvyrcahi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mvazhskf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2inmwhnig.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rfccprsj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2unagwzqn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2czbonjrq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2eeumtqet.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2nfiznuxg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2elpymkgu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zhoyzkxy.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lhejzizn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hsiwlvtn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2vxuaikhu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2bnznimkm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ujwvjmrk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2nssnrigk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fxjsnlao.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ltxyycjx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hvkfupzu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rjpxqrbo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2hvdtizsd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2aqhrwvbh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bgwyvpne.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xozpknwx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rgdupeir.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2kpvsioos.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ykxxeldx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lbkihoum.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kdkmualv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2yqsbchjd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2htoaibrb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kmwxxuce.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2racjkiqf.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2egowyqiq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2moiujszf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zncxfsmc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qxnoskde.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jyloyqxq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2upfpmoqu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2izzgilud.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2vzgdgvgd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2tffmcudb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2topchegt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vdykmsxc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2kjzqajmt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2jwqycrak.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kmkgvaid.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mdibydwq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rytfcqxo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2gvwhfken.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2flovpces.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2jnfbssrt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2tpzqbikk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2dbnvkklu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2axunzvfa.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2nwoawcqh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tocvaisd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2uigzmvyq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2woavxmwk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ovfilkwq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ossewzyb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xvxwhbsn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2luzizbco.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2kqyikjud.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vxyqlcur.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2dqqeftzr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2gunescqq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2cwqzvluy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2itrmrjed.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2knbbkkci.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2fpfbsbns.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ekghxqfv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ulgnwydr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2tcgcbgim.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ivmewqex.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2kgjlbykq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2berqtarf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2dmxthynd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2bhdbeirw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2dafdmqow.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ghcmgaxo.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jevixdgf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wvdhmurt.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2aqmemvnm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bfubegii.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vwftphau.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kojqacib.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2oyvyuybg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2udefczlb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2stmetdni.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2mqtxgdxr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2eogymamz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cmbhwknq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2codhpeqg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2oorpvfrx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ahgxzllo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2yciemqap.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2qvxjcdcu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2wdmibfjc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nnzjumzy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rsvohxnz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tbnlfheh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fpgtirmx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2nknbxrhb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ujhgaxto.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2vuncqlqw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pqpgzgfs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2beljsfkk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wnufcqky.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qtkvpwaa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2rfsiutlz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2agmpukdr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2bqmofvzp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2qssiovvt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ccryamgq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2xnseftmw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2cwmrzvmd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ksylgymw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ifkpogdu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kizqsmcf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2uyjfwbck.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2stohredi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2opvuhueq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2axfubkaq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xaknlhxo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hrhfrqpw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uazfjgfr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2oupwiqoy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dqcrgdqe.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2gcweiriu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uamqmtvc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fmgpvbqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fevdizfb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2pduxqjyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mgpccitj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kxdbfrjj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ztrakyrl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jksyqoqj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pwhoqbhd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fyzqkvze.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ikoiippz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ouvwppte.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2gbznoinr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hdtduodw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2viwrkmlk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2aufalhho.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jsggvxrq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nfnzrnsj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eqodembr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xzwlxqgb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2qdofsjdn.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2mtcytikz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gdmjfzpq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bsckrbfv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2mzzlbdax.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zmxwjwfc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wkucwfmp.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fhsbfhni.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2quhvflch.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2giroidtt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2elniskuk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2gyshtalb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2vwxixyri.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xpkeexvz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2gsuvtffl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2gykikpum.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2svjqahjk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jjztkhkh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ednnzlla.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lfnayyct.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xyckbnyd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2iciyfmyc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hcphyraf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ejpevdmu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uxlbsibp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pphafyci.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uklwidrs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2hydbjjxb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2acbzyrep.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2evyutnfx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2qypiimxw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2elrmvred.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zjykcgpy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tunocuox.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2egipbqby.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vsqxjros.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fevzqozg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ifggkbpr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jaacfves.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2fvodxxvu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2lulbhokk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nghuwdig.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2mdlegjkj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2dyjsmnkp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2biepqisj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2supjzoxg.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2dgpuejsy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2slxumkjw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2vorkkjsl.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2hynzoqxr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2cfaqqaps.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ridqdkuf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2doyntggo.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fysesrmg.html


<!-- 参考信息 -->