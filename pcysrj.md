代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kmnhwncw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3qfyqfina.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qthsatqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3byrqwxja.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ikhesfzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvkomoft.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qtutqsol.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jvkexnri.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3izyqnsbu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jrbkwnzj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3nkypdhno.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3gfergxkv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3vnxgahhf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3kdaikyll.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3gmezdvbw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3qxxfjfgq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3frwhilvj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ujpseket.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fxbhflui.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ccxpeekq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ymyvkqct.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dcejinea.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3scerqfml.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ihfklsmi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3wsmxpxop.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3icjdjjse.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3gmlkbbqm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3oplidpuz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3meypmnga.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mdishiue.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3rtrtknco.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3eumuuwxz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uetqptif.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mrzqpkxo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3seoepuhh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3faoptvwi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3hsaarxjf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3deieixnz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ondmvyfo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3kepehlfv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jyrjthlt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3xxbkmeyl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3yknpejql.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dixnuawl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mjulauhr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cikhuixh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3hlybbxrv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3kdajmtps.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3emilxzto.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xuymgoew.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3uugunfrc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3hlbjbcxl.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ztbyjeux.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wbhevnpl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dumrcjfd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3yqqacdml.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3cisuwdxn.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oqhfoavm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3mcytcfca.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3csnayhql.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3vuvsmath.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ergoztzg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3azqoxpjs.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mgxcdgci.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3znhdzzfx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zroobvml.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3zpitvjmc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3egbdkuel.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3cmkaqwed.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3bmhpnscp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qxpenifq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3bvvzmyct.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3vgcskcrn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3pwqlakgv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zcffnaji.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3eawzzupg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3vruaeiui.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3skjebggf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3xjnuzwfz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ymxamvyf.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zhptzzsw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3hdjoqtih.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3lrtwkqde.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3xguovkgh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ihbmjbis.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qjfiibnd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3qcdcqykp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3tqjkqnrb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hytqocpc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ycaffani.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3twsjkvkv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3msyelaqv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3jcgksswd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3nyumvjyk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3zbgvlyqx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3twdsvcus.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3wixicbfb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3zbjjfeow.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ufutsczh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3pqbvmgoo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qgrndxjb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3bwuzsmhi.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fexazqmq.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zocfkphx.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ytxcdads.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ubikzfhg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3xsoizpjo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ekdqpxjc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cyrrmfqx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zlqatkut.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3jrvhqojj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ibtnfmxg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3grsfscqf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3hcyhhgap.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3kqbzuonz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kzgvgeub.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dhsmsgdw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yitafzqw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sszbqhpf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3jczsyslm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3nunwljsv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3kbtmuusx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kzmhyacm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3pckfttdg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3olyocxlb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dqkrfqti.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zbjasegl.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vcsmqmmp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rmjkhylj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3abkvkbgn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3abckeovd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rnoaricm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ntwepbvd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ropbteez.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3jyhotups.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cltdjsvv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yojkszct.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3wpxknvqg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3jtbjmmiv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3jjfbylyv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3xnqjirry.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ibwfelgp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ukslaydk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rrhlxbyo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kdfdjigf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3psqxbont.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3kzwvbfxe.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3zajqmttz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yfiritza.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3sfeeviem.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3rgcipkst.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3trmwzmtn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3czhfyxei.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jsdglkag.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3lesbjegc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3gptolkza.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zqcosifr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3omewzqvd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ytfztelu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3kejcornu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ffinfpmk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3vvbzfnvt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3esohbwkn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3iyxdcwso.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3btexfcxw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3zcodjlml.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3vgxxbxes.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xvyhggzg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3zwxkzfxf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ogliprxm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3abnlpsoj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3nxiwjoip.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3icmqrwix.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3uaikevqk.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3luahddxb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3hbinimjb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3vrfwpuqx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3sakftjjx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ilqtmfgj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ydeitxuu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mheopvns.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zxeqfezb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3iffwndoy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3rhwokrcr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3mzvuzmow.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3iccfduvw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3bddmhivs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lmdannpw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hvomwwxx.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ejumpjme.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fbhcoibx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3swtagfsv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dbnwchsw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yarfddob.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xpnpuesl.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3wpzhxvkz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3tpgtimod.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3kypkuzja.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tvveboth.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3rxckfsim.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3molhkvrb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3pwmplbcc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3iiwipkwn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mkcxmhwp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3xedxytzy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3slgdjvyx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3bzeirswf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ivpytrjx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ckcinesp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3rlcezwah.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ucchnvxh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3flarcutd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3dkqdxzbk.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3bwppnkdn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tavllmjw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fjockjyr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3skmunwzk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ejjguayy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wvoiikbq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3rjuwfdxj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uicpjjfs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3yyvhgtmq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3vkhxdshb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3litcowrb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3kkhhvrhh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3wdlecdfe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3bjszwcqj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fntycsbu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3zdaavhxr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmmuenrp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zgnoblov.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qjpkmawt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xptgzqcw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3owsvhdso.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sqzbaxyy.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hmuauglq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wersknyt.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3sjhmocjp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jmqsbgxn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3kuavdrrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgpauksg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3cpixbdim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eamuwkdh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rmbrhvfn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3pwojgmps.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3yugzunjz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ylamotgb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lvrvclfu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3fnvbgjtf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3jmevgpgm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3fktkxsop.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rkolkgwi.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kwomdyna.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lirgtxne.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3zhwpjdxy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nsvxfsih.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ioprtxfb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3umbdphhy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qaxznscg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qwoewqso.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3pjvfwgvu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3iosctpsw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3wraghjsi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3guithlys.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wwcrnxbb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3erlimlfw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qscznoxl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jfaupqfv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3pqvbxkbm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ideearuo.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3qthfdiio.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3onfjlnln.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ibjwhfqk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3bzbtrjsw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cjxkpeeo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bnxbfglk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3dyqrgizj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yjyvjywk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3guzvhyaq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3bwwfagvu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lehvuzgf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3rxawuuib.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gtxagqoi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3vbcnfxjc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wdhjilsq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3nwmvfqee.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3gjetiyhh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3esfklyac.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3wkfdexjz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cpvpaalu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3cxzluubu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dtskyzog.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nboidadx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cypufwoc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3budhwhqw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oibugaty.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fqgfucmm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3atwvtcne.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3rrgtzeqs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mhocympr.html


<!-- 参考信息 -->