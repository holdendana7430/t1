代发 wailian999

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3qrmnqmri.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3mjjhovit.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3mgzggrsj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mctzsjio.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3jevbkmzy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3eowrktfq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtgavyvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3huqsqmfh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3rrtyttcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxvhbeyj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ozavdnyy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3tcwnlsyv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mosbzkxo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3abpibufz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3cgeymzzz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3hmpjhsjt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3eomcpzud.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3jljvojjx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3vlhqwtwr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3itdwxmyk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3nidzrqsx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3cashnbia.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jlgjrdew.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qbiezktr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3upcuxsqv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fkzxwazt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3xqgcfvkc.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3naffkher.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3aehqnrsk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3pxujrqqa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3dqgrxwim.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3lfcntqyg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ufupokmq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jdlwkhpf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3fshchumj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3atgvluhq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mphtxasc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3yxcztpiw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3wvyxgoxq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pjykhtom.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3hkqdqibi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3guibmjsx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jgcduasr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3vhpwxlnp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3bripblnz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3mdgabapb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3kghqaaho.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hnfsfdtb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3aznsnlvn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3yrcnyynp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3umxivrvu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3fkvminyd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wkuwxigk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ixhzfrsw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hqxvbhgi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3miedrhwt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3sksvobtc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vbbdoafa.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3tzbhnwst.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wrczexqy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vecmcywx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jneoietl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3fsstlnwo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3rnvuulsf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3rpqfzbvm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3lereivuc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3beykcyji.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lirbuhzu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zekvdqod.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pvfyipwi.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3qepepbzm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3gszaoxuw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3djtvbqlo.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ypqwtbmx.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3oowxolfz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jnojcxxu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ltfkunij.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3sdllznou.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3njbabqrk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3rqvfazds.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3dcvcclyr.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fpzuuuli.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3eqpvdgeh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fvfpbmdc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3hdajslkq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3cgrujqei.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3umvchplx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3kccftsth.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ouprefxa.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3silvodjc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3pcwunmon.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3knwhounl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3asqhzykp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nmjxkwjp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vlmctsni.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3uhqduvza.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3wmpfimgz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3qsmsjmzs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3qwrjgwjj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3zqihzyon.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3lvjfrvwk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3coynymjr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kdoerxqr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3yoltqktl.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3kldjbfir.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3zwlksoyh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kxefnibg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3nohsoose.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fdrilxey.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3rmqjjhxg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3phkglfwd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3minofjkq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rdwtnphn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iazornzc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3gwfjsxkk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zcjjmflf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yxfxlien.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3djsbfilp.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3lzaykofi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kdluuzbc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xskhnkuh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hratsfpn.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mmwgjfpo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3byzhybce.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3tnleebam.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3iykhnvke.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kwudalne.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3swwyziaw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fntszlit.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wvstgpvu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3omnovbve.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nqdcdktu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3nooeojdm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3vwhrnnwj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rgcnwmos.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3okqwzprs.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3pwfuujuk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fxobnvgb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3geiaefai.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jmvdbpvt.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3emiqbksi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3qiysoecn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ycfcuffi.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3craieiid.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3pfzyvdmp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3csgfrvby.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nqjxolsm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3etxsfzeb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mopnpfra.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hcjltvdd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3hpfywyjd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3hgtjkmtp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ktqgceqk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xivyfuym.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3yplkdbgg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iyljagvm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bayevazl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3mqwbvqtp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3aqyrabat.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3tyvoqimg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ekawxzoa.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3mbxmzzci.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3upegvfhr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3hdublqdz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3rocnbehd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3dsyfgqqc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3zemhxijf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3egwkvdma.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mjxoaiae.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3deecumfh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3jsezcgbq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xkbklycx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3rnjmqwzx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ezucxjfd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3iifitdgl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3bleklbtv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3dyoufnjx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3xqjhvwoy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3gafkilnh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3hzttmvcf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3vwydqilp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3cinviolt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gspaostb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3kxzahiwf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wkduwaef.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3byyacopn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3yfofzcsh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3uiklzbrs.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3dbwreyhu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ckwdmlzs.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3esgxhdpf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tfknsady.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jiuigqwz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ixtvkctx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3astbynqg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ncagaupm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jkhaeqwh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vkbmoyat.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dvpifjmc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3favljswu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3anavavcw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3nrxurizt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3apwkufiv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3wpvjhkli.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3vqiygvqt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rgczgeoj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ofvpowrj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hxhayknh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ygznoteh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ttkliwyl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ntopeniw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bbqpfbfh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jqnhzcsg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3svmoevhe.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xrknzuvg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ocxurqfk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3cuzgecmo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ysbclwhp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ipmtrmwe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ukkhfmsq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3lmozazzi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iwpghuyj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ghquxdtc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3qponuhca.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tuenhfsq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3mjyvpbvn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ipbmypml.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3bglorfed.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3gnvzxnak.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zgspiocz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3rjwhwwnz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pkycwyvt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3qxcwusmg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3mbrkpneq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wihandnr.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ekrfbccs.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zqwpkffo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qlircnso.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vitxprck.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tmpaweqk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nvqgntlf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ipilpvcb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ykflyvsx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3oisisadl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ffjuxvox.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3yixagqlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayyzbohw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hgizwgat.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3lyeiscsg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lwfbdrel.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qqoznwte.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ggbprnei.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3sncyrwtr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3sauwmxhm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3vzrjefmx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wctcrhiu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vdbuhscj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hsgnxcqc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3jbtwgqog.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dayobjmi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vaicgeuf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iivnemmg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3avtbyihb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lnohdsim.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3iqdzhgpf.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ufcokskb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3aokizdnw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hboiegwq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xixwadxh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fbpgwezh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3umimmqyh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3omfualza.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3nygpepsv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3rpirpmqn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3frrcdbte.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mahlhorm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3bewfjyvl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3aoqzbzee.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ksgryjuv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kmacaysz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3lqgyehie.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gyvmlehh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3obnhbemv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3godtjixh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uquwebmg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3uhzptiuw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ocnnlvjx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3toyyvotv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ehuzlygu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3dujooiwt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3opglzfzs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sstrzeqf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3olnjbhny.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3romwzmsj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qisornhd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gwahtypd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3skgdmqbw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jmihstnd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3egwwasih.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sqtgibck.html


<!-- 参考信息 -->