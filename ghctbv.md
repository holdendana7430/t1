代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3scwvxwsz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3hrrkmoth.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ruwditsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wwjwvrzg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3mzgrepau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3owejgmuo.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gpxekofc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3xhjynkow.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dsulujsb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qozqpmnf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3rerqjlpx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3cwjmlghs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3higmsids.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3yhbfiaya.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3unuwtxoa.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3qylwaney.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3obpfywjw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3yysgmrml.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hwvuwosx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cxhtjnyz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hopbgyvn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xmmxkddj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3vntxwtge.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3coyemcnm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3btbgxrwk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rfwwshir.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3iovezgdl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3lqxhemwc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cimgazsn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kiilmdqh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3fpbqitka.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3rndwxpty.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tsmbkdol.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mjgqcluq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3fbuwxmqs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3shagceur.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3nxdylkft.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fxibebkx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ejaviggy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3tpqftmii.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3wsrqrtaw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3tzgupurn.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3leihuiyj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hlbmurzg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3csvahpcn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pslhpgvr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3hzisrcys.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3dbgeawxr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gjvskhkf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ksmyvnli.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wddfnfct.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ekkzjngc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3alvqtgbr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3szlotdot.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vazvupzm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3sychipes.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3mrjdhrav.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mfxqivsm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3efugjpix.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3yetnaoda.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3cybsrwlm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3daeyxjqg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lsvhxzjs.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jvfsvxwa.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qmaqwusj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3exxkdlgi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3hzxhfmpx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zdlbbodg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3meyiamvb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3fanzkapj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3asrtuuhg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3hoeoggpt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3byjconmm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3gwyewuex.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3cwhgzhla.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3wtavqzlj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3udqlgxbt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vzcxhjuh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3aciclazz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zweboqpq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jqllugev.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3bmshjuxn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3wcypjjaj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3qkhirqhb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wstdzona.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ptdcpgml.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3hypvvree.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3scxxwsck.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3itdvbuqz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3sckhruuw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dsogomkz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3wnzkcuup.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3sliuzjre.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3tpdpayge.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3qeghtofa.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3wioogndt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3xtpgpckz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3zypnhynl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ecnsgtky.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3pexflxiu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cxwaktdq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3wmqbrtxg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3trhgrkxb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3fvhrtzzp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3affghhkv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3jnoyhwbm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3sshwvinz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tzmsibgn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xhdixsfc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bupsgwrv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3wotijgpb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ytrpclpo.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3geukdcku.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3tacserxz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3yeqedckt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3mkizezxq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rhnplbuz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3citcyeqe.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3eqkmunlt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zoimajge.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3akpxisgt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3yvfbdisg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vipdarqh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3svafdxnf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fvhpmucy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gwyprpcf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mqkokoeg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3csxnohcd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ndbpkaeh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3dbjdjndc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gakyujpb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3adbwcenx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3cibltocg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3cukfcwse.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sdxtwbwj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zmmnqbqr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fdxcpmph.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3dlmsphfi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3dylgfwzw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3sydvjszg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3vtsiumdo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3gatncdit.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dwokzlsx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mkaqftnp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yuoyxdcm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yrqcfoiu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3huallrih.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3vtiqwqpc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3invtdzxf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xfafcpfw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pmkbvwxz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mftqqxua.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ibwjnehx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qxudqeui.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ycavtaqi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ovgvujeb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3olclgjil.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3dphawmmf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3gguabonz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3cmtodsqt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3jfvovzvv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3jgchbcip.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3jkwksllf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3zaoqloil.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3relzgbfu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cyinoisj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3szwsxywc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zhkgthgb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3xltbldon.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3xksxfohf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3phuxfbgi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3bzcwdqzt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ilofdiyl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3tqhdbrdg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3bwpfkxyo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3zasaugoz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fbgskgjq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3hqofaybs.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uffqnoom.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3wvixkvcf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3escenvvl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ezhztmvj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3incrkjkk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3czkaiqzm.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3hrhhllrs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3atgevpvg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ujowayaz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3yfpdfalt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3exekxupo.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bibcizuy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bejjjxlq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xrkdnmqs.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lqqkiurc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jjifluxd.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gykxqcin.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3lughvcuw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3fjbrxpdh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3rmfemzmo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3agehtpda.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ulphzxhj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3trjjvsat.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3uwtkrccs.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3xgevwfni.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3whqmqoqu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3qxugzomp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zyvtgkbu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3uzxlruxh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3prhofhem.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xfgixsrv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3urxfnypv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jlwexuoq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3hjfbfznk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3dxozakop.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ppapzqcs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3uezgiufo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hfvgosew.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3htctpfql.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fyarmlub.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3jxhlzqyc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3erqdqpcz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3evwzucmo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ftzhyeiz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3gwempkzg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3dmiuszlt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3aqevfjjy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3joowhmsx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vtfcydax.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dkroywxa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3fqoarboi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rbywykmb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ucmtkeyo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lnhfgocl.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lkejpgdf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fulhahiu.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3djolzjni.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ubvvqgsv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dbnbuaec.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3uwzkymnw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ieikkjgk.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vlwpnzos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvolhwfn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ctfaoneu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhobznna.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mrblmuol.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3pimucqnw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jmfiakdz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dwalgtpm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3janxfemq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hsptvywf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3vomooupp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3aqxpiqar.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3msntcdsb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3urrnuhss.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rmiqmoxw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jrbkwjfr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gkdzvhid.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bkfchsjx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ewajldvf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qzyjxwqq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mmmlrvcn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3fguigujg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3spfzqiqw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3pplbrqfj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3amxkfzes.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mummjamn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3msypwxpx.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vkegkqxp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ahnzvxlw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3larrgjcz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mocgzbxt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3mrhxxjgb.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gzeuvwck.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3spmyejvj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3qezcznwh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3emjeowgp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nidskien.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3cnfgmstf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vmlhbdop.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zjbhfkip.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3nzlfgvgn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3rywhglsc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3bawdbyhw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3scgsnonu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3kjuhpduz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3iotlmoky.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ffytzswp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vedgcxll.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vhydclad.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3tigjwtqw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kikkjmyg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3aivojtkk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ietowhiz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xnsnbahv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ljicbngm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3muubbwct.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ytxtsrfi.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dafrzsaf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3cfvqsipy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3hnpvpabu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3krexmezc.html


<!-- 参考信息 -->