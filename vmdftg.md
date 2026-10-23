代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3aoppueog.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jpxcbgrk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vqpyavxt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mjanifgj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ttrwrzfo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vvkytafc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ydrpgsmm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3jpymrcss.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3quwazwyz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gffhafsx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hcllqmgs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3qqsissvf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qkasduuf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fevjxvfc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3obeyebwf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3pkhzdtog.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3psknbsrk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nvvafdrl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3qfuustkn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3duunrnpf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3odslzaxo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3fdgdmchx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jfagwvgs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3juiyxegm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dxheukyu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ctieukxq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ornmzbau.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rqrwjito.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3igfpfnve.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ujxgxizv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3pqxdppav.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3zupqcoms.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ysdbsqqd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nuubzdak.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hceahdje.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hbblgvsc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xyfpqgmk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ehqxtcpu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3oqzowsja.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nwpweons.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3eabaspcy.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ivjyagnt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3zinmxvli.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ccqtoanl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3weegfwfd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3upqlqpue.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3llndbjhm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ehcrtnux.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3anbtosel.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3soyqygve.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3zcyhbdnt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3mvckhttq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xylhezlw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3uvjkpdmv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yeoatnkr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3vvtcinda.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3itinatzs.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3quycflqc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yvddhuiu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3yquubumt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3watagrhr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vvaldbrq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3hkdascpp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3dqszuhvt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pztwiguu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3bjyjgpkv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3sjzhbcjn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3xnjaqbmc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vguchwel.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xqtksggr.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3akthrrpw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3uujrmvht.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3thxqflml.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hozxdapv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zcestbjh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ulkgmfgb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3adhtcenv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3lvkxecsa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3czabzyjp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3dfxiwkqh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3nzwmalph.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3hcgumygo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3reltsylt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3lowegxxz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3xmtbtjon.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3nsuswpjn.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zdwixtwh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mjecfzgy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3axdvqirf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3clcgxzec.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tgfjiixa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kqccmmeg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sajrkroh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hnipsgdv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3fzrogvfv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lrbcpoty.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3tsmhhtcd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ydyrvnop.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3oyhmeqrz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3huoiqsov.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3govlzswx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uudhspbn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zzamhhas.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yzgbqfyy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3sekaxxcx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3tvlmiyou.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kqdjpqoe.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3hlibodtu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3edgvmlpz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3toyqctab.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lnhltwjc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jdmmybpu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3plsovwpe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fcrqcvya.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tqmqibkd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wqujnjhi.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xodpeihq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vqwfrvhu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3djawrqof.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jibfppjr.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3acbjofoy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3bjguuiub.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qgmgrmhp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3uicprznb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3vtoysayx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3sbkisndw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3friodgxd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tyzmfvff.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yxinhxuc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bhzlwujn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xhteteld.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3yxstpihx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3bwzcpjhm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3yhvcwvou.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3kaemqofe.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nywgpsnr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3zcbesbpq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iqmehtsd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3injdleaz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3sqihcugj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qdoyfwyd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3rlarurhx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3jdmjkdkw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3scpxwzur.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3avmjsazw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3mkmvltes.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3qyagopjx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3skiajeiu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rdhpegmz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ngsmqnqc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hwmfdaay.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tiempqsk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3vaskfejk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3jsikbjou.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3cwyjhoxq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3duvxzwvp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3pfjjmynt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3axmficie.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3pyeerbyd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3okidadzw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3loxiwhlz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ygfiwqpr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pkkigyko.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wilajwkv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hvrphywd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3urrzdqza.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3lkqqpyts.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3dzxxqewb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3qyayzvct.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3kpbltqtw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3tkfxutso.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3sfezxuzg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3qvuhdoju.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qauadnlb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3daynkuzy.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3albbqibv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kdgtzkxb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fpzoomiu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eshvkwdb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xdqngnps.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3lwjpttmx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3bvtvyhnf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3pvifknjx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3gegopcxe.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3dhnxshzw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wrkwvpja.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3kihtijzh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sescmfuy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3gidhcgfu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3udytncyt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hmsplqbq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lelekiyv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ulyhzhdq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3vfzszkko.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vacpcrus.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3zbmocgwl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3aaxwidir.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3uqramkgo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3lbtzfjic.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3fqqbqdlm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cygetmmx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fseelhbk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3huijvwfn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3qdimfrjv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3alloekgn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3fwfdqnyt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3jrqqkjqn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3voomeehm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3idzicaqw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3juaearif.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3bbfwplae.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rapqpnsc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3tkcfmmuv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zpvhqnhq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wkjrvhye.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xeqpgweb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nqdqajro.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3eemznkta.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3aieszdut.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tmdculss.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3geshdstj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xxhrklbo.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jvtficqz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jhpihlbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smeeveno.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3cdjuiimj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nzlrstgg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ldzokmlc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3hswnhdop.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zdxzqeco.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qowyukdn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3pkiqyzal.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3osllqdlv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ipxfrgzu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ogjxabzl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sxcymfgx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3nnvioprh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jkvlnoju.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ltbiuaun.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zjbafurj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rxcakbeo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3byjshbss.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3leubqlri.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3icrstvdb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vkouewuh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lfxzddal.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3tjskaosg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ggklxmdy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3znomojbf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vnpbonbq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kxycfbpz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hsinsjda.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ktwaeiel.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3gentdtsa.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3utxvgiii.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ltdoewdh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3zqyhycha.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3kcapsqls.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3upfncthv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3osfpdduj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3gcrthjlp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wcipildw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uninnlds.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3fkazemcp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xjnqapvs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3zzkwpdma.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3etwaxyfh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gehbfmdo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ouplpuja.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3mzuriabo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iiotcdlu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3leuuxsja.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3wikbsveq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3flcmlzqx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3pvjtxsii.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ctgmqvgs.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wbwkzsgv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ethpqesf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ulyofaoz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vslmybul.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ngsxecci.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mlwrmilc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qptrrzqr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fnrtajqv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ropcxfmp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gmnzxqxa.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3zctspkgf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sqzqpnum.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3gqvcdiiv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3glaacxuy.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3azmdlmsw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ghmgxwaj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3uvygbisn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gmjzvikf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mgpvyprn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3bfwuonlb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3zcmozwnk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3oynzjajp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hlylmqoh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3nxslvrcb.html


<!-- 参考信息 -->