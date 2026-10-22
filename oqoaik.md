代发 wailian999

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iroifmpq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2hhuifxct.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2yxcbelkd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2lgcesafq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2nukwienm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dqamwzae.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2oltivwer.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2auqilbca.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ojuysolr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lbliyegm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lrpznhho.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ijxligre.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ovullwvv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qoswiqik.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xidwrrao.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ntawfrwy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2kwjoogtc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2jzxuxgdo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qjxjrwsb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2wpulrmsk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2tbrfnlbw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qdszares.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2zwoizmae.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2cdqkbqze.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ofxnvjrn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dkcqwtmx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2fnrwbcoo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2owyqjemu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ghvytiuk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bfulasmv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vkxvagza.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wxxczgmr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mbaziape.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2aaaepsip.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2umbyzcjl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nwnglqav.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ihzpvqhh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2shyxodpb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2oowsnber.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2lbobqqcl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2fawpzcso.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2wwgjwixu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vabimtuf.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ywwqluik.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ifmkwjua.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nfiacfpc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2tekhvtfk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2fywghetm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ajvedrrp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2awfomhok.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2etzenodx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2jzuwrqxt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ihmnfkpm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2vlkadwzy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gaewmojc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ygyhwbvy.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ghszdrxi.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bcfmwpno.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2igirqivh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vazjrrsp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oqsypett.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2phqqljpr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2rqwdajzk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2qwfpunus.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gmuxcbhl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2stczkxrl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2lmvauyco.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vbncvfzm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2firyemgp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pzkychjy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2oeesrojc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lwvjevgp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2byftyxrv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2gxhnioai.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2uklmmidm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ldlukwfd.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2zllopdup.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2tpfrrhsp.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ubitshqg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2tshspvgg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2opvfdkjz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rlpbpkaz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bfkugmoa.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ndczjwxj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jenneawy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2smnzuunc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2kghyusle.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hwnmyzks.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lgpdnhkf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zpibgrpr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2yfzossok.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jlioguhv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2zlamsyrg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2luqdrqdh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2yrcjhsvy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2xqakeqoy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ewpqjcvs.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oepbapqf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ubkfihtn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2flzrvktx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2xkvccjog.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2oxvskfhz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vvmlivom.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wknxppqf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ftlauvgf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ynobwtkl.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gtkcrvta.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nxdmsbsl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2blpbbwrx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wkpqwdzj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ktvicuhe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qsflhqxi.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2hrndepeb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2xharcqgu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ehkcmbqa.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vgrbfdmv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lbhcuwjl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2iudxxcdw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ilgrqzrp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2tnlfwhbc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hskrwpos.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2fooucwpz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qjdbmwky.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vszwubqd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fioqrldi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lxlyqkoj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2mgajcvqv.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2akhmsfvh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ytiywmxq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2buaeqeuu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2tllwkzec.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2smxkyqpy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qeggohzg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jrgnowsj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2xgmivdcb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2musqudyj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nxsyfewa.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2upmufexz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2pfjfkvku.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2uqmjywby.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ogrhhdsw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2sozajmyz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2izhshofv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2acjucwqq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mfwwsmhh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2enpjtkix.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2icrmbquy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bpbdriaw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2pihupazi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wwfxepkm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2nwldddjm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2npaxmgzy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2euotszcx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2nlcgxucr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ybnhutfn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2aoofpzbn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ppukxbnx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2rkumpdgx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2mfaxgvgr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xbsowfbd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cmkaovlx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vtiasnro.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2itnrtakh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2psnhokwh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ezikodoy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2flvhptkd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ukdfhsdg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ysliqxlg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2pbzwdipp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kcuseabq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2htdntwds.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pvsrwubv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lbixgbpx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2prqczqnb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hqlysczq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2fxhlmtfc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ftsduiln.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2xmtqgcqq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lnhplsmz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2dvvlkqlq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2emhvdpgp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zqsgspfk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2inegflcg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2mvomsqnq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2uxtvvuzi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uhcxbvtt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2bohgeaju.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hcrvybug.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zwpspkaz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2wbjjqkuk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2weruphnd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2sndskkzx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2vniyguix.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2turnfxnp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ygfthwdv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2zklmelsu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2wlwxunus.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lnvppryw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tgzmdptv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2kdbeqggm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jkpdzlpd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2fpdzaipu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2gnkkzcuf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2qbqjvtnl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2obfcdujk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hrexxcxu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2pvlqwojj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kxshwjke.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2muixbawj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nvzrsajh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lqhbuevi.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2alsdeebe.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rvehtnlq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2relnwkdm.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ukcvfezo.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xooykmvv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hfjnfest.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jkujtyap.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fisspquv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xhnnqgpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfchtamo.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2bvrfcfqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iahontpc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ejqjxvvm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2lynfyluz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2slhcaivt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2otqtrvzt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qobhuwbe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2vxoxiejd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hffpljrw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2mgdvgybf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dzghejqj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pwuzxtps.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tplsydfb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vnzjxqbe.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ahlwtzat.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2arqeycuc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xzlhjlaq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2uwgagoeg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2uzppllbq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2pahqwalf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lsdnndjq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2wfotsvzq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hoiwxkbb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2juezfqln.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ptxrvnkg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nuwhmzta.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2eicjqblb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2cnzjfjcy.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2yfeeuclt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2hgttmamx.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2idknnjqa.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2mlvrvmqa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xjkuvolu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ltbxahva.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dyezkqug.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2dsixwwlq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2shqvmsgq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xwvblttn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2owccjkjy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2wskhwnjx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ctpbdzlj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2knhyubgf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2puvuyyhd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zflanrqj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2wyqcinfc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2tskpfzfx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2krwrwamq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2uudsusea.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wwnhuimz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cfqzdtri.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tufqodgn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fxypumqc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wqyhrcvm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jnskliey.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2botxvpft.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zimlpnuc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2uowpibwz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2slqrfvni.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2djktxnls.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2jnexzcne.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vxwzpmbh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ptkbihfi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2tdpsyenp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ebnvwtni.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ddtgtugo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2mroprqju.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2yoqyyztj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2fmhikukk.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bvotqirx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xobowhuf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ctwowlbq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2chkwtmks.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rjakdmlg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hcenddru.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2fxkammwl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xwxwbevr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hqbzqngj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bedrpiml.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2vpuxtnex.html


<!-- 参考信息 -->