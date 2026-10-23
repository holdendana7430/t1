代发 wailian999

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ewfviugj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3fqnvykon.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3oeoyxeip.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3exsnporh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ksavdrad.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ivmrinag.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3bzhkwawi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3waomtaxf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3fbvlwoqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwnzmzuh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zgoxglob.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3dpfazpfu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rnepndxv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ndnmrzuo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3didaqamn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3mrjdzcla.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3fmykazov.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3kpuqgbto.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3xhvfnsfe.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3nofpkvco.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3vlrjtqkb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3uduslrhq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tdhekpco.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kyiezfxg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yqgptssq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ehamuceb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3maghalla.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ictrehpo.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3bwfalouq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3szuehceg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3gpeprdzb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3okdywxrf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3udjytvke.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jxlrolig.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3eaohcfbh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3warmjqsi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ycmvagsy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jppbcuof.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qgaonfoa.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ssvwbhog.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3garwpmyc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3oeiklgyu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cvkodudu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3nvwxslby.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ivxzxyfy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3llnfbccx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3tzfnxhpp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vnossgdi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ywbphgfr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bjwsmfnl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3dbdylvxm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3nsanfuwv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nvdtnihw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zdktwmjp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dopzxsoj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3seproehz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ngrjheyv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ajuqoleg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3lwioynhz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3eqtzuwpt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3uucnujwx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3oqnpyksp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3sfeiznvr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3kkkaigxi.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3zczhvbdz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3jpcqmjex.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tmszhmmc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dmddddwl.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vmswefil.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mbnrmjeb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3akfpbgla.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hrspqgew.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ctqvfhlt.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3plbfyejc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qoyaqrbc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3rncbbfgd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3kasurnxg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3jyzpkluk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3rkzccxes.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3sowymjsw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ivuqhply.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nwswgojl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3cvqkhulo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dhnkeusq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hjnokglx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3xyhgrwvf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ovcunort.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3paqwlykk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ipyvnzrn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kuuhprme.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ullieiqn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3qtzsnnta.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zveneydx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3yemrmqxc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nwhiucmr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3okrcfgcc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3jnqggylr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3thsuwats.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3wqczdjpd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3earcfdtw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3jxuquwgy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3tttlxfyb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tzhvkone.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3xzbeeigv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ygmvvrtn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jwmpsnjc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3mrtcrier.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zjcbkeja.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3dddyzcyk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3hncftqhc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3jkldqcyt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qxgmbkzd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3nfbucyup.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dcyolfcz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3habwfiqz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dqwxuxyo.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3vibpisyx.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3taenygdw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3qnhoupti.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jzrmtmfl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hootbwau.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dekomjbk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3zycvunnq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3odryqyxf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3tfyfbtjg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3zubwffuw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fsaiwugb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3cjtlhxrf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3acykibfl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lrrbttgy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mbgdztro.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zotbjehc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uacoeqnf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3tebpnxgh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fjutilfk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3noxvylgz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3mzzxbhke.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ysvvhehw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3htnamugq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wbuvlled.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yykqkqvt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3nrkxmqfi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3mpupiejd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3wsfftdca.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3wrvufwfy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3lgaxndql.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jxuwfvdv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qcnqpkdh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qzpnjpyy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3aviuiqjx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ukrjcrww.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3hlhmtzyq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3nvnhhhan.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ahcbemwl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ymgnxjvu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3igzsrprm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3fnrwezxm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ezhpbrhe.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3fuuejqrd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hrjsuvcx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3uorrpjty.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3mjfemoks.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3mkmnbbfm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3plepules.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3bvqwnpva.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3pwipwbmm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ovpvysoo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3epppcgyb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3jkbvvzsb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xgydjysd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3mfszwmkj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ezniqghx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3tcacqmdc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mlxvpquw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3fdlrnnjw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3dfgsrvcs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3drppqttm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3fzjfownb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3jvlvnzdz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ttvgymtf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3xxrrvsjv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3eieyszjp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3dnttosdp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3vezrbmgq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3shysmmhm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3khnzyrib.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zqiqrskk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3xcumosvd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ymiyufpe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3krlvghqn.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3szrtgoxe.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3aewruuef.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3pxomineu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3krhzvkjv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yxektcpq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rcgqxrec.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vfzuyntc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nemmfzou.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ecrhzghw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3cdsmsjwb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dpccfkdy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3uzletmbf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3nxkytnap.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3qaiadlkc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gsnbydcr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3kiabmfnr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ndfouskw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ypqroook.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ynxpwczm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ouaxydgr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3njktnaje.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ejojakwp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hgbqgbay.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3bqkmjjey.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zmymvqry.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3unlwumem.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3zylsspll.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3cbeugknd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3qxdyatmy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3pdcbhbkb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vqlqaywl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3brojcqaj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ergkosos.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3grnsoajh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3gqllmmte.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3gbqidfij.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3meexoucc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3asueloei.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3aprvnkgj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3wiknsztn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3leahxfhz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jejutesr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3xytdhpur.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pizwnlot.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fcievucn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xwgahtdt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gkdsqfml.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dqvqyxly.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hnqbqkhz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dvyifaup.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jzzsjfue.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wwbvgzid.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tqodflfe.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mznczdyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxzfffxq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3xjbmwrwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iuugkqbm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3utlszsiu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3zuzvtbra.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3kccbxsml.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sozipiro.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ynarhpke.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3gwfimvzd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bwznotbg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3cvfdoovt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fllhddnj.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3nunzszgc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jynfckxz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3rrjythpq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ahkyccwv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gutupxvu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qbjpgqiq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3imodppcq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3yvfumcek.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3dixujbgg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3pjvosciv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3zvadqqrw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qqiizvhz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3erknvblt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xqxkzytn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3awzoxnur.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3esrevgkh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3evwabgxn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3fscudkyu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3dyumuibr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jteeofbs.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qdkzgdua.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3bqsztrgh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hacyqfnq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dvsdqowa.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kicqwjwe.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lirztpoz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lbbgyhvg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3nrcznfox.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3olqffxjl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3iwoiyxzn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3biqgljsl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3stkhcddo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dpjutupl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3jzlsizou.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3zbsbkcwk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jmyxensq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3jjpaewma.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pflomwjn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3fzsatmnb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3brmcfise.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ulrlympw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3knaexrfs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wapeivwb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zhovbpvv.html


<!-- 参考信息 -->