代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2baoidryj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dpgndspk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2biqauypp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2wthmcavc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ppxggbyx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vmfbjblf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2pnckesfi.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2irjxdpim.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2mtdjflfq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2qodnlpup.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2iqtrtepg.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dbvwvjkv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ajtpmfiu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2vnipmkod.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2dieficqp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2salzptbf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xjpzswhp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xjgvgocl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2nsavpgnh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2rwhdvywa.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uwsgnsqt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yiwablaa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bjsrsqge.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2oyfelziu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kaoxzizi.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tujbycjt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ieluvvwt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2efovkwrr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ongvidcl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2jaruudug.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ossvrywh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ejxpczbk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2cydpnjci.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2hkuncwiw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2urxwwylf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2iqavxgoo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nkzcvxym.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2aslzkwcg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2bkjpnevi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2geozikij.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fndrvstt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2klhbczcr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vkgyogfw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2stbspklb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gbllkecg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hhetryas.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2sfpnublp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cpuljrga.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ljhyeoeg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jpmgpetk.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2kceuwkbu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2bkigeegj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2iqhmgykv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2kogrlfaz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mdanitig.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mzjfabuz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2meoxykyp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sxraarly.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2deveuaqe.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fecfljlb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2korpgvkf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2jfmgcgtd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2xdntlwsp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2hrymthap.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2mdjsmkin.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2omlnlbim.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2sjhlgmhh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2sypmjukl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lysdtpmh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kerxjbsc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2einvkouq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2areeccfd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2oecuhnpp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2qoudwrtx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2rvhmwghg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2cvnqvlpb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dkktovdg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2cpnfgscy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2kvvgkaor.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2lzgvdnja.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fiankchs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vagkqpyk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lwttjdkh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2osbioieq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ebspghgb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xmvhttay.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2hiyhbrbd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2vyknndke.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2mvdgvzvh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2mtdeyppy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ggloplze.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2byjatcrq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2zkidyrcz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2zmtwmiyo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ewdgrtjt.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ckgedzhc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2whrhhrnr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2havquabl.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wjndbngf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rdvicyko.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2pwykqkll.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ofygrrpz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ihzoifna.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nfkhscxa.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bhnoqrij.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2hvpysvfq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2qduoqzzj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2mqamlehf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2zfwnatem.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wnorifxg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fhhweddb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2vkxcpzrd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2qkbupvek.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2iljaoehi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wbnbqtzq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2rqvtffdp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2obeswwpn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2arxrtlla.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lbjlyaml.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rlimbhwr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2peguazjj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pyzaphwd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mmyocqud.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fkpbyqfk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2tdfwuxyx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2twabpjmr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2fynbecqb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2oipjapuh.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gxhxgqpp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2dkjdlldj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ramrpjae.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2skveghbz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ieittfph.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2eyshhpeo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qjahirtg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tjupimzy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ewkvtrcg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uviknacu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2bvkbgmnk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ekjbwhxe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2pjpcwdnq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2jnzpwqkt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hogxdimz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fianuabh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ozlyiusr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qipqpnrk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xphcudaj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qdwhnoah.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ddsmppxz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2fulfhuis.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ejtdqbsa.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ypszuygl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2moipxxqb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2okkdlqup.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2dlfwddry.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2pidwqyad.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tlwbrhlz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2uozzwspc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ifexnhsw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lylygcyx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2siptildu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wuaahfgt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2nmnkwtbj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ioahgisz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cexnlwum.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2hexikdzg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2rkfbilij.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2cfadcgmx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2nylwdvvo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ymllcsqa.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2orjhvwgz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zxvtanlk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2idbuoylq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hazbcppm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2xmiwgsqq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2xercsqvt.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2zmknecps.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2heipcxtt.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zplvwfkg.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ljhkoefg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kpnlfovp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2swxrnerm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2awfwrtvv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2phgypgko.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jealbvlv.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ozmxxuiz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qsjbomdx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2bxyzkroe.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ezgkeecb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2dyukehfd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2uqjghszp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2digclvpe.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2scdzmqhv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jlwnqvfw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2zdwkbpzx.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uaozxsjy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2uztcslpg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2osrwajdd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fydzinlc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2heblnruo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gsmsielv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2jasisotc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vsaqnmrh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2hymuanto.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2axgmqkfl.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xnouhbln.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2whmhdiat.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mwylivis.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2fjtmastt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lljmdrng.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2zmiwnpwo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jxsigqha.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rszccgjj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2cfatltxy.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2vgjplpas.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2dhgtdgby.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wosoqpwo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vvxjaioy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2efqdyfgi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqiwxoua.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ijyuprvi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gnpdooie.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hsgyllje.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2flsfzpah.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2fxqizvfl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fxfdioqc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ibeszldz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dmyqddtg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2adrgukvf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jfrztnpo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2aizdcykg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wusmdvon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ollfpjol.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2azkfbspi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xntdmkzf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bofuxghu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2qlsjbztn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xkfzyuxi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2txzokyzp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yoovgian.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hbwgvbdg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2geinbpjm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2puuxpfzy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hxdxxnsk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2obhzngvp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jojixfaa.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tjrabvch.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kupuhehu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lglnlkds.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hacnzyxz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2rihorlke.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2eilpfbnu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ijhozycq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2mpebnglr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2peeyvvrc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2frjljdis.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ybogsktu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wslupawn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lqfpcwwd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2sjgqozfq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2nggydlst.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2prpywfpp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2rurxdehx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dhzawmjr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2fgrmxztl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2mkazvqve.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pnvfofpf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ywokrihj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2heokmglu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tpdawmji.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wvahoblw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2gxumvqmn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2atjpcftk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2axvnoknw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fjidzxxx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2spzppsjt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2azcjefmm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2hzugshqr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ibqvawjc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aapzqnqo.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2sffutzll.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rmhhjazb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ijridmnb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2syfqjjgl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2havgaerw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dknpxaxo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjxbbrwr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wsucqrje.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nmqmxurm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ufgolqrq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2uwhekibm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pennteec.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2rdtfluto.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ztlojfaw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2djgzkmmx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qtfqvbis.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2hpqgckce.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2zxhfbcms.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2zxcldyik.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2fxypwdxj.html


<!-- 参考信息 -->