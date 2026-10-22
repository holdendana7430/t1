代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2uurckcai.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ykzekbeu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ekzyjxmo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2zkzzjevw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uktqvpjl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dpjtqykh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2wgztdbst.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2nplnihue.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mqfofwao.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2adegcvrv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2vvjwghsn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ytnokrvz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2gtydoira.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2gyyovopf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2sqkzwpuo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2hicplnys.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vtdomkxy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2zdfwpnyi.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ajiflxvq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fywyyqkz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qotsfypt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yanxvxql.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zifxarec.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ulvjlnlo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cyizovbz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qaypxqwz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fzbpmtwu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2frfcffmj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mkzlidzv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2iberxdxt.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hbikogcc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tsgrhwyq.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2mvogwpnj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qttjzcgf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2gxtxstws.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2afobmhdl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2kpklemww.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2xdmhsieq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2aqhibnes.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2txstmyzt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2orttuktl.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rowzbnyc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2kromgsrf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2odqotbse.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vcksulld.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2wcjwdija.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2mrosghkf.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2rjmuvuah.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2lmecxpbd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2isqyvzpt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2rpyvzhrj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2tslxqwpu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2cnrbeqrf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rslmszxf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2bbwwbmii.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lwmeracj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2bukakqmk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2qtvxnoew.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xqiadihb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2bmzuvpit.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jvvmptxs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2llgpjddl.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2zbxijzvu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2lkksegnw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2abrxsifk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yzlxgtpq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ofdkkfhw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dacptafq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2eculnzes.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2iapswkcw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2xrcfdhln.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2cnuoggzp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2xlrbshvr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2cwumwtyj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2vsfkmfnu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ihspmfxq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2wxewbuil.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oashzogn.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2moisxyya.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2abfemslk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2yydybivk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ihsraqih.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nfhwelzk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cssywkil.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qbudsuog.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hstwmxpd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2dantxrit.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fetvzgmm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dfnrblgq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2xntfbtey.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2zqwemrca.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2emxderlh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zjefgyov.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aavwikmz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2yrudnccs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ojjblrwp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2dxkzvszm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2wmkllnhi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2udbfbioo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2kvdlztmd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pbfuzgnf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xmmnpifv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rvyjqlvd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xznitvnw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iejxmyee.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lphvkrhy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tkxhynii.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pblknkvv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ygnhaubo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bjhbwcaa.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xshndafo.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tdtyartf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2iiwedpcq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hyhujvkj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qjojmbue.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2gmnuiyre.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2fbqvpjai.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ixzjimox.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2grghcixe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mldwclgx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2yzhjyqyz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2myriphgh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2bgfpvrzt.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2fjoshpbi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2oaikljsp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2pljhgfsr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2surrtobe.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tkyckpmx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hffqecyh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vklwqjzw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2uupdzkof.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vbkfzzke.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2awppuatj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2znwtsysh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2yvzmmsrw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2nvahbsdq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2cemiqfak.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2jgkveelh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2blxuunxw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2zdmwdtdq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ehmpzwym.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2qznwwzba.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2wrxvvziw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tlmtombf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2fwklxqak.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2zutbcofy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2krijmyhx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2kzazbcyh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xdjloqrr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2whfmfjkr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2nyurqzim.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2suftyknb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2wdwiqcsz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2asdachko.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jdzfzogr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iqggskjs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2pjgordme.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2eqpueqlu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2nnhgkyjz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2llyyuhpd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ogxewdpj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2fmjygqly.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2cyxyfgdz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2iqmrtalp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2xzxwpicx.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2znevjvep.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jesihjza.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xkucmlkq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ineaijlk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xynkpcxc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ceimcfzc.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ovvxnjfq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dvfauazu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2wzunrbhw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2vxvulwft.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2vvgfbjoa.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2bmbsnpqd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bsvygrcf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2dhdpmfck.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jvifixbw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2bkhvmmpv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2bqngmcws.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ioornoez.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2clwjnlrm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2llnuvktf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rjhfakyd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dpdvotht.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2rzcyfrtl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2lufknxpt.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2slqhgfhg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2atzifjqc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2nwfstplq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2slienwql.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rlzkfoga.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2heahreww.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2tnngqbjl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2mjkrvdwp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2dtanvlbw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2woclmjnx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2nlrymwrt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mpxufutq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kotdcvvc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2chlyfybc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lmveyagy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2vnnbmlae.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2uoyfifzi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uhkpbgwr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sbhrreoh.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2jgvtifpv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bueojxja.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sbfnphkr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pggfpxob.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bzhyoifh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kkjlmhdm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hmylyvwe.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ccqzqnop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjxtpoei.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ysytubck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwyqamtz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jrbzgith.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2nqowioen.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2qyvpgfcg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zrztkpva.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wvdgzrtc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ygfnoqdj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2whwjlumr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2wlshmidr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hkxcyvmh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2kottjpmq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cqlssicm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hgysybwz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bjkfflin.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eycllooe.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fxifpndo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2npjvwyin.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2anrynsvz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ktnigmdf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fwbxsrpk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2mujwkebw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zwwdevfz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vgnlzhxv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rvipzxxr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hljownbc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2agdnkioi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2yoanqqyl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ygtmluya.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2azvkopyn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mgtnvqih.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2oiokosfq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ymmlvyhp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xbvtbijx.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fdlvsqvn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2htmimyzf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ynbhmpzi.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dsqwtnff.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2glulkhli.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2mittaivr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2alalorfe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xalxauek.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vsazjhws.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pmahhydr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2fgtlogsp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oewmlsiw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tmqjgssq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2yuubygcm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kfefsfcr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rlyaapcr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2blzorqek.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2negsdfop.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fogemclh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uvtgskfa.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fvuhrddk.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2csmkfcjz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qeeqeheq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ocqrqzpn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ujucmnlr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2fotwfdqu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2osuvmwuj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jrvheoed.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zffpaqck.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2myncakgr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2upqseljg.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2trajygfy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2tpvjhpjr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2mjuykwit.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xgxlmqpd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nfugvkah.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lefjhzmg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2kmtcthqk.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lskcajbg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2xeuqqdav.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2cyyxewpm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pydfldzu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oiljknpv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ncsswlat.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ohfhvaph.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2yclgxkru.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2qcgrkphr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yyrgycdo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qwrbupuk.html


<!-- 参考信息 -->