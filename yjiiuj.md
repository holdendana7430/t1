代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3bttwoyrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhgmrgar.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3nbxppjqp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jjapeyyn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3aqizyeap.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ovpjvkub.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ixinptzf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3kmtmacub.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3hckkxbwl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wfemwmpm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3nfvrmcse.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3lnczxdfh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3zgsfagld.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3mbtwmmna.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bebchqpu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vxtsqxus.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gkvrwmxk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3wutusndm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3wsoqvtvo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3xrkheynr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3hkeifmxx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kiiezqln.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3htexaivw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3smazfakp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rlnvusif.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3woutmnmw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3lihbshyu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3bqisiwdh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3axywbezm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tkkbylrp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hkbugswr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3lzvalhxy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3bpddultl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3njojtvap.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3crvxzrpl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3rpljlhli.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3wmckascx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3devyctmi.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3cjlejswg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cauodfqr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pvkjifgg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ipyerwxh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3wgskysom.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3vouknifv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vxjyhtnf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ujhaeuvj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hsrudcpl.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xmrjsehb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vlozwzby.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3algzjosb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hauiqbij.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ojndbltb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3xbxhvemx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rpyimmdy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lmgvmxqo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3qmhbtsis.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3qunotlca.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3jciqycpd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ogrypxpm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3holrkorh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dxdstyhx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lriqvybc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3tabehbxi.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ntisxutj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vmhphjog.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3auswjvwl.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ugzsqrga.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3gxjdxrwm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3wfvynzhb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3qohwhgmg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3gslqslap.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vikivcrz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ydxypgkr.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kbworioo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3apimnuoo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3layphniq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3roswyabu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3xczhlqwq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ubwffduj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3frytvcyj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3sjztjnyv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wgcmlaai.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3mzinpbjp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ytzlcwft.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zdngobql.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fjlquwoo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kwsdsiim.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wlerbsap.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3daisoegp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3oraiqanz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3hkongwto.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3vudntmhk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3jtbdlvmm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3jlyjvexk.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xjqapuet.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3bkmwvdqf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3sgshyuox.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3xicowtjd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nzjrdjdl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3xmxiqubh.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cbfguppj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3gmwhdnom.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3muobdpxl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ighoddkj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wpygzhmb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lvhwjaow.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3iwiiiccf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xirgrbzy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3vqyxqhaw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3cfxmwexa.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3qopzhbep.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ypecmgqx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3enhedfhz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uxyhdcwp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mamjyevo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lxmvflla.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3twyzpsls.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3qndtiuzn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3okcdking.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3gbgwumae.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3zwogfrmd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3oyipwrbu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lkurtlkg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lpfcltxj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ryvmczxd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zpejxrtm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3azdbexsh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wikfjjig.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3xetnmehm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3yeprxuqb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3vqiubbyk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kkzxlaef.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hmuacnfn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3khtdnkbh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3xzvrumfp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ufhqnajx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ydfhugoi.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3pplhnveq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pyzaoloe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xshozgib.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3umpdaqib.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kliuosdz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ozvmcavq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ozhdjwyi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3eoxnrenc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3hpijtbdm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rkfkcomn.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3obdhxmge.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cbyrmvbv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3hktjlqdh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xfzdmjyh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ujmtvykl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3eggmfusq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ncxmwlck.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3kpalqbpr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3cirokcdx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ubcsonfo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ikgtjeen.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3jauprsok.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3yrgcmhxw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wvxkofzl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3gjuoqujf.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3vldgtfsv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rrbinpik.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3osxfcxfg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3rqosrpgg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3mjekuzbi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3jtyuhyfq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3sxqgabco.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3tprxvnyh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3wgxkfifn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3xmzcetsd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3dtgczhqn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3kmjmvtst.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3fnaivqod.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3jryyqvzw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mqxcirel.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mriaazaw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ewzmgksx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3massarig.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3qnukkegw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3sjxdihpl.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3tgbvfqix.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3bkohbpvu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ccdtpjlp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3whsregwa.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3afklvsfw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vzzsvtdq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vannqrid.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3waplgscs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ethhivpz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3hubfgmhj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ycrzwizw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3wepcxpwu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3orfrjtvh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3hvkgoixa.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3eldphtbf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hmaqmsdo.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3obqwihns.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3utnnukoy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3gdjabzhf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xpdxjmhs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3kjvpfamp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aifqtsar.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tvaeoxrs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3dnwhidwi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tjeintcq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ixotiepj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3tcyfrwjr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3fzfjqrcm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3orgozpzc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3pieoavsi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljsokylj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iysufkre.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ttnbyqwq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3cyocjijn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mdzjvvud.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ocazqrjn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3xzbwmenz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3iecqenjv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3iihoqbzx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3dkadqsnm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3wnidbgrp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3bqbjhoim.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3pypnvdaa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3uileetkv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3eoqmsnst.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3jvybybjq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3rzxqxrkf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3twztlryt.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3katrhjis.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ctyqgwwm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3bgxejlbs.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gcdcenit.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yydlpbyc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qpygxfjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pqsjmqfu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3kwnyvnzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njsoufag.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3geemaihv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3nttuavyw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3wsidheqx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3reasztvc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tafgeegi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3uljupygd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kbrrnbrq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ercjfrld.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sjnyfydr.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lxxyjzrs.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vjconamy.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3dwvlcumq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dedoqlkg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mwgynbss.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hojnivar.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bijqcidg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mousntxy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3czonbrct.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cwjparay.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3vlevjyep.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lrcifmws.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vhywkaro.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gendgleo.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xgatckdf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lkmjxtit.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3uovtvseu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3rqxamket.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3krtvgkof.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ucifyamh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3rgsxxtnw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3qhjzunku.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vedfcrpb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ackmyalj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3kyetalvw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gfhwnsji.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mfzxumqm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3uccshott.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3zlxcozpp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3hnychwws.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hnrzqhar.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hubcbjez.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cwfqfybc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ggyxwyhf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wwdvuhky.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3elpwcsxj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jtsmofab.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kytdjmna.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lludpmxg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nfkohnvy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uarbcrjx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zzygjmmn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tyjvkfcm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3daodkrjs.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hqfrwiie.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3huecfpbv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3bykcmryy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3grxcgzak.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3uppeyuyp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3xgpnzugd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3zqmvsrxo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3pjzdnurs.html


<!-- 参考信息 -->