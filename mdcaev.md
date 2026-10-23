代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3bofkutsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oxbcpqff.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hrwuxnxd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3tnyrkwsv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zkhczglp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rfbygbtu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3igpfshsf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3znmodtiv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3kolsqflr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3wicgkmvr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ocwnaoxl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3tcxdqeae.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3cvuupxyr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3klsyqtcz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rvyngesm.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3isjarvfw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3umxpzdsg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3obxqnvfp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3arlpiddx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3cgvjpmad.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3fkahffwi.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3zqkenhew.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ntwtgtuk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3pgvuphzz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dffclowy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xnvnlngv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3olwbcaje.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3jdcutnxg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fohtmdoo.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ibyijkoa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3zeucppxr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ycqvzkdw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zepwocga.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xrkdrllk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3vewwtjqd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3hnpgajpj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3dibwyvjd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3zooxmjpl.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3vbrpdyzy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3aubhvwda.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hejbkdon.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cooidtdd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vtjciorz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3wfejzerz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kbpchqpp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jwoubwuc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nlyvpkye.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dsnoddhn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rucvnjwz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hetyedgu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jaqzxccz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ozunmuzg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3zoyqvqrk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ybmznuis.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3chmodlgq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3vgcpdemo.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3hemdwtrz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3omzvlqtm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xbgudokf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3trlyhkdh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lhxablgl.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zymkyqyl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3xuaulsir.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3cbgpckke.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fcdpbamc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3aqyqjeiv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3prifzyen.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3lsvnnvhk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3peqejvob.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3zvmakimb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3pszjfvbg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3mughdoys.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3cochbmrt.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ovygdpae.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3apgftxkf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lsutoqva.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mzbbctqr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3tfkczidt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3pbokuabq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3wrpwxhtn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cyzvnsky.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lcgabxxu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3jyhavbnt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3rkimnpbj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3knsjabea.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nmujxmtd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rjdndsuq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hfpwvied.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3elcizsro.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3eujdznwi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3pcskzufm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3nnyjaafe.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3egfsixhm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ueqkvcpq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nhxxcaam.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3jneotwla.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3lulktawn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ovszzzgq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pjavjdeb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3yabnwhaq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zsnxmagm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3atteqqoi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3vmarendm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nfcajjei.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3shkcpsxl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bwxvprhe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3honnodsv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xrbypqjb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3uidqcscp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3xnrjwnze.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3dxrscbvl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3pqhaqbuy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3bsvivuis.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3glvzuutl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lookxltg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3atdgzfqs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3gwjbqifx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3xfnmnajn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jezjrxen.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3vaxqzgki.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3chdgravx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xvmibnmp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mbwypgmx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3artrxuyz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3teutumzz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3sfrrvcli.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wyuyojat.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kgaulpbt.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3bvutpuil.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eikctemr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3yaqvnffd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3uzeepjsl.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vutujndb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3chhgmlzl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3poyoyzkx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3vebidinj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3xaawhoei.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3vynasdqg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dvtxzlxr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wkcxcxuc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pdxvstez.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xlqyncld.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3qmocktcr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3iorjcwjy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3jcnfbhqc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3bvogaugh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nwtayqkp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mtcltygi.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3boxdbxcj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3twomwlgo.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xvdpqomn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cithnnoe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bnbpsbws.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3qrrhbeou.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3feljnakm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3zzfjntqk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3qbpbmufi.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3vjxbyhem.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3isitnnyt.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3tjxaitvn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3jaatxkzm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3rjbrycyk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3glevbvwf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3djbsqjch.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3iyxdhmhk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3qoavepsy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3znmeamqe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3tawdztgf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qrgiwbbg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3tolussvj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3jrggldjk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3hbnvplit.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3znsgworq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ykuruwzy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3hyzrlrgv.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3maagpqbk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3glyuquzm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3iutfncor.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3wcwugvtr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3tobggysu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3owwpslcm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3arhicwwx.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3cipboqfd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ygatbebu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3zctjtzxg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rxpifklr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lyeegkho.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vfzwddog.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3foybxoot.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nqtgvebx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pbbnbzlg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3gpkpvztj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3gjbaspry.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ujynjegb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fjavyqta.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3byrsytmx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3juxxpvph.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3izuamxtf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3crfasylt.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3gulwzbge.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vwexurdy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ufnlpfij.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ucwadqfl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xzjkemgv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hiiplywc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3kflgbqnd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zbxhwlsi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3buyrklgc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3pqopeity.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3sltybulw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jhpqdhnr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3egpryajy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3kjqtjzds.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fqbbykpy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3gfwimpga.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3vlpubbvf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3iqmgxels.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3vsdcrrto.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3gwwznyzf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3tpprgrmv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3mserinny.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3kvozhddd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vdnrfexy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ulqnmdrf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3fdqtoplo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3udbkoplj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ukezciuc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mppjxxxw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3fgnxkbdq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mxvlijud.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3axdfjpkh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wxdvgtmg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dgmovvcc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3gazxmvdc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nlnlcmso.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fpokmzbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3byecofnl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3lakmpegb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3blwotsan.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3alhswnwe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3seawaewl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3bayblzwp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qsvulobb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3biwdaley.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3uslziigg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ndojbmam.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3yqsvvnmt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wcpqyjbp.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nfrqctxc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ucrapzne.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3micmnanf.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jwslqgoi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3joxxfbzj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bfnpsfys.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ggklyykk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3osbcpuwy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3zhavxchm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nrxnqfkr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ogwfzsdc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wjehoqaa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mivbgota.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dpmkpsmx.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vxoyhcae.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kczjzzbg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3bhwbjfci.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3kxaaxzcg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ffbbhgru.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xiuenluj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3kgidacpa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3mmlujzwv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vxcgaotf.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xnliypnd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3aolvnoct.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3uklkeyel.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fghddtlx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3eogefwzd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ewrsdhwe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3egpdckmd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wbzatpcn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3inawthhv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dnjhvkcy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3nkjjcjaq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3dkdinfpo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qvfoxpck.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3hyhjidko.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ggcezsvi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uihkmdie.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3byxonild.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3elxjmtfb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fsktmxls.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ibzeekpj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3waboxglt.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pqlmkkau.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3oprwslri.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3jivdmgjs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ugnpsxcm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fbwcstum.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wogcmyjd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3hsexvytv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wvktrvcz.html


<!-- 参考信息 -->