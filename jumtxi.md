代发 wailian999

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2czfngsmv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2pzgsuxjg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2udwsgmoj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2jcwhckbl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2whyeursf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ptwikvxr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnzotrzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whrwihfk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2edfgghsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zajpfotg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lmswvywc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2wjjwsdzl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2pgofuvmx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2crevcjjh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qkfvixty.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ttssskhi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2jzsifhem.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2edkrhevd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2hbpskhkb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2bbadbwll.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2szfingoq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tennxqaw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mulymwtq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gdambqaz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2mxsdwwcf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2dmklxsve.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2tjydrfbc.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2efkoptzl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2abprgkyl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2nkhrzwai.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2dxhtlehr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2fetdhmud.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gqyhqrtg.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2abeqjati.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fsezxwmq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2jjmthnmh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mhnnbwws.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ilbeuroo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2edcvdbmq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2sapsobvh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2olerjucp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2wiwvespm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2djpfyfeg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2bfzlflea.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yolrgoqp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2oaxfhcgg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2hlugfnqt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tluozjhb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rmhqlwct.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jwkmlieh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2xpzarujc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ujvavqdj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lcodbfgo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2crrseakl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tcjaehjh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2sfchsefv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rxfddzia.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2unlfcxwr.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lemczpjf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2oxwcnqpn.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2iztuivpb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ewaiidjk.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ttnnyfaj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2rooqvlqn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2heemfcrd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2bqamyghw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zxcxzfsh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2uxuzvtyx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mpueexho.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dnhuzhjj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ctcphiwn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ljffaajr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ypellmml.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2imjxfynh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2yhjyyybi.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2cakcpmkb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2iftzmgjj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ubrggybq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2glbnnpmz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2nckhzidu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2fyjkptzr.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kxfxlepq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2wgxnhujy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mizmxmwh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gipdaypd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2mhzvzsli.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2xamxspij.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2yeooxzdt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nnexogep.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2brufmmtj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ttpifxan.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2konaywow.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2flxcunlb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2walqcqak.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2keeybtgd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sknlwxyy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2gxzrdtog.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2uloxlbxs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2oyqbsidw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2trbuftnj.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2muyzxlwl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2phgmrvgd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rbtvcznl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2yujylagl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tsdwxswx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ldaoziqj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2icsnlluc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2qbfownlo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ndliuxfh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2thjpvstb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qmurfdwx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bupubvrl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sefagwbu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2boqxuylv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2wfhigsgt.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vsiusbnr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmlhluqf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2jbadqszo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2namzuokt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2exkxgasq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nfimyuda.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hifwbqgv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mgljbahb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2gtnpppng.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2czeewesg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2rlbjkqkm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dxfqmfaa.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2niluhixq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gzqcomvi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ptaviupz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ogtfuqoa.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2orwtforu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ixhdjlfu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2pidjtmxy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xkvyemaa.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kfupxvzj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2pfkkjfyu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hfrmjsiq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hzrpcwrc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hvgkjdkw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ujpsztaj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ayiztijx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2cfhmjyyr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2tlhrkxip.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2rsbtaxji.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2uxopmsdd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zcvdlfbp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2crghghyi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2oeluiqpr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dxqscxfa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ebjcrvra.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2tesigors.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2nnulugps.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2tsadltqg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2dwdutjie.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vkhttpxv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2lywnivsy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ybcwwary.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2caipacfz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zltatoyt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2imbqdlwn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2serupqvl.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2dfmvrfgj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2bhvpedfb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2kdzowaio.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2rhiwptod.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2trtypjmd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vuffwarl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ogbgvkza.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2rxgemwvn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2mbpujzkk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dqednoak.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2vggkedpo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gbqxbipx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2bggxbsdn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2hiddllsy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2chxbhlgu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2tacepvil.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2szigqqek.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2qsiovvzj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2zltqpaii.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hejgpcfd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2khnkuobj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2xarqhbne.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jalutuja.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2azbyhldj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2teovetwn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2fnamyudn.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ovutpqez.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2amjmlqam.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2driimixc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2xlztxktw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2kcdztbry.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jvwbxzkq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wxzypjxx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ptqvqgdr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cqsurzqj.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vquvurzg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2leblithc.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2rkcwnkhp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hjtgqvih.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2qrndokmm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jnluoxbe.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2vdkzsnwp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fadewest.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2zwivkysy.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ettorjcx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2pupbpnlp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2hlkpqsbk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2vaencnbe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2sgkmcyrn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rzqkbbuc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2weoqnesb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2afvecghx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2razekmvt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2catkhnqr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2wgudwbwy.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2wzgqbfbs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2srqsvmsg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2iojqwexr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gzbzuwok.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yohfyyte.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ifurlfgs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2trpredcp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2pkmgwfkk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2sefhrdwd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2zfnziphk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2mmmkofso.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2yamuiajk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ethwrhff.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2lgeygfmu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rmhymasc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2yaxhltaz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2budkrxxr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rdybwyid.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2cysrjzli.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tnncufxe.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ycsifjid.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lphacmkd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2npvknxvs.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2aqoczqdz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2wcgxtfoi.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2slqwvubl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2pnbmqagh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uyfzvchd.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2zluoeyqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mttpahfb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xtrlvylu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2supuhoee.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2rfrwlrih.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2evylrtke.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fgugruzm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2rkadtkkp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2jeadujtm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2tcrkmcnl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2czheiqqx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2deaghuzr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wgtphebf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2xdpciqdu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zcovhkon.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2umwlnveo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2iujrznwp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gdwjykkk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fajaddcp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qxjhzgjt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2iiqdfuld.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2qyhcgccb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xckeukdp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dhroapmu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qqtuelkq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xqnjmirn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2nwshtjce.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zxxgqylo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nexyslga.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2agyakctw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2icolqgce.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2jifzjdua.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2tocqxgmj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tudbjclz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2azmiukms.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2jlrdepiz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2oddrkgjm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rvxvqrvy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2vafatazi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dzndsnke.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2pyhpwvkw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gxxkptpj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rvopgegu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uobsrugd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2aujkmxvv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2okizstex.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xengqodn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2yhzpuuqu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vqnxexkn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2qudpsklc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mqrhkixm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2erzgybye.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oukolowj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eiiacuwv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hpohrduj.html


<!-- 参考信息 -->