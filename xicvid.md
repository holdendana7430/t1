代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3thvethuw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3jecxsnfb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ggqtpvcb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pldjmnuz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3eirzdtxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icijggqz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jtcgitdu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3nnpverpj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ckaxncku.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3pxcicdiv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jhlhnqvc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3mfcezhcy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ioxtsjqo.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kjqwlbbk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3xlfmzjfw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3trzjjfnv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3zttiyddl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3erctvhhq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rzqjobgc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jruecrve.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oqkpvlwe.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3psrgyzqc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3sqcpxgde.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gsljnsst.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3gbilqwtu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qhcesykl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3essiakdy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3grxmxrqc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ecygeztc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mbxblaed.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3cmmyfwzm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3zghhhjvb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3maggjvqa.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3cahfprvf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bvbjijrf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gqehyddu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ayyupcwp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3plcsnttf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3rvatochb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3lcvxqhcp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ydanapzt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3nkkptipl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ldclxkch.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ocuyfhrh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xwzafvvw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mmqsitys.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3aygmfbie.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3lfronocx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zqqqinso.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3meavnjvv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mtigjfob.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wcwmuefo.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pufxvrfn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bekodsyc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3domdzucd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3sropjfjf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3xyujajqv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dxzjrnmk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lrtfvtms.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3suaedbkm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3serphjbd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3oucboxmr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3isasomgg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3baefdfud.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pjbldomn.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3osksdzsr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3tuqzxjje.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xekqlwwu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ikajqmhi.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3tvdaxbns.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3rjhzuyrd.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3onbduami.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3kqosmeai.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3rigoxllg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3itqqiwqt.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3rhavbrck.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3lqxkqkpw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3njsrugkp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3yxoirmet.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ienbimww.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3uppcsoqk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3tywtrstb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3qagowizs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3wbuubtqw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hnhwvlfm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uoxzthtd.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ijvndbxh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3fcocfuxl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jufdevqu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3agsmrbnx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ydrivtrg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xipqfsbw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3gkukwqja.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3hvnwbpon.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3tqgksqft.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3zewvbqhg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3nmkathsy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mnyuxnku.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3odjypdhv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3wksksdyt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bxsuamjs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3qtpqrrgh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3fdghohto.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uwrtgkca.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3asklvikz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3wpwxkdrx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ukyumnzn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jtfktffb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ggeldiqu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jjrrzykw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3fcrfkyba.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iffqvdqn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lwjyuwch.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3mbzrfdwz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3knhnisfs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uemxjhaz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3kkpgaboe.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dybbtwxt.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bzdfojna.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3mhyauopn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ekcmaehc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3mhzilpye.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uiwukchw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3sptkruye.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3njnenlro.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3movvopmc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ounryygj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3emliwcrl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3qlidntjh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wzxjhhcj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rzgupfll.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vikujvpu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3liuazvrd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3unsthciq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rfawtxpu.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ianotrlr.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3tyzevril.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3jsgwqbnw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3rhppwrdy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3njffaeyl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vphwucpr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3nahphlpp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uxhbrbcm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jrkkkykv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tklflcrr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lckhdkoh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3vdlkpsbs.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3raurycvq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3tpmtojah.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3skdecvnc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tqdxbnlp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kfkkzzcv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3kjvksarq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3avuvqwbr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3demgbnbj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pllpxjyg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3buuaujzg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3xyfhqbrq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3bywecnkv.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3pnmvzlml.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3icdtdmeg.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3epwtbtkc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3oewpkgdb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3dqribltb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ialqwleo.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3tyoqaige.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3upishogr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qjujoroh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3sbgtcqpf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ibyvugzq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3yhfaiian.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3pwpjgzxg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bbeeoogv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3prnffreq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3jsxtffoi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3wdrlpiku.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3fwbulwkl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3azdrmdtw.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gcofnaer.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gpvskfmh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3iesmfmyt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hjnmywfu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3nxoziivr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3rrmhqzwx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3abxzjxqd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3tuqnveaw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3zferinpu.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jskjmsxe.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cvdskvxz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ldbrsbft.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cbtsqavk.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tsadnkjf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vxksyggi.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fsnpndzp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3elygllbg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3wvmbytgz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jvwwlkjy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3mvfyzpcd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rppebrzr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3uyhrmyst.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3zvwggwea.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ueqgurnq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3mphmagpw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3klcfnvpl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3mtvaufjl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zpdoapql.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lqztcqdy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wnktknnn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oafhysuf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3pxnxzxsr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3sdenpodg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3qqhnhnqv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3idzbzatu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3cjcawhkh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hcpfbpec.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3mhpufyxh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ksacgykj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3roquitaj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yytasqig.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3cfciuqve.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3bcrmwoxl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3eydfioam.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3iammdurn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3symgjbuy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3noyphpef.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nyyszqls.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3pifyhlft.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ctfgbufv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3fkmyoodx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xhtzwwnj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bhxuanwx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sgkcdkpy.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tyczbkvp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gfuglxzb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lunxcygi.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sbvzsbxe.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jjfvjtob.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3zgawkmti.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hhlvjooo.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3eirayzhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pctizwez.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3jbkusowf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umoqwpim.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rysrtgsk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3akuxngwt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qvdwswoh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ixysrudt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qldyxxiv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3zsvnipez.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3nuesdqer.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3bavtawfi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uprfarkx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3dudnewkz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jihrfzfu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xqyurufl.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jjcweqpq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ixgmkvxw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3urijfrgl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3mwmlzjka.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3orsdhsef.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nrlbrfvc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wvhuohqm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3vyjwajey.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pkpdhwdb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cldsunll.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kuqluddu.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xgoqtyvw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3phoqokrr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ieddklxh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mteiubjf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jcnmucvw.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3npfsgfgo.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3nyuhyskf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ntavvpwv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ujelfrzb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gepztvie.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3iixgrjgb.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3figecdbb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vehwuacj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3hjshuhft.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3alyjulhk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ygkcpqaf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yxirruzl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ypfcxarq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vqrkxpfd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ahjkpsqw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3hlgefreu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3avtnxyom.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3gtnjcqon.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pvqxywih.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3qplibgpp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vivqxiql.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hqfcjdqr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cknxmrvc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xonhhtlg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wvrwhfzh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3saqghfoz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ctyshxku.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3zppwobje.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kflsyive.html


<!-- 参考信息 -->