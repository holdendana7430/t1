代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ecydhahf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2uggmqjdk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zvtohbts.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2swvfkyxc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2rnpqfzvn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2pcefrkzr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jnhrgvfd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2lhjmpugl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2fnaqmkry.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2orjnfiec.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2usmgkfsm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2psqnflmq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vgjnsdsz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ygkndtsw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2lfczowoo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2pknuanfq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mywikloh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2aczovnnt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rsymmdkb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rnaswwxt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oyhcihoc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ltlhsyjx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bncjpnry.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qzeshloa.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2eugpwhmo.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2voaxqwqe.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ievqoect.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cjfcxxcv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bsebtvha.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qjxtksto.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2lvzpxkjv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ynjyimmd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tepqbqay.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xykaabhc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2chxgrhdr.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2hkdxjlmn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jnksmnrx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2tknghsds.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iosejjvi.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2nujzzxag.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2uelpfnzy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ymysejcy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wditiiwl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2chihouup.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jaoeqldw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gkctkjug.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2fzdfopjk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dwoelfsc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2aphozape.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2mrwqtvth.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2hvplnqzu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2pxwgwarp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qwpgxwfp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kbgwzfwx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2mrhtrsnl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2tbjndixl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2didphwbq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gkulilrc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qggpaxbj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kufjznow.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2snjyssuk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2vdthgwvm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2cbmsdcot.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2zevnscza.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2nedxoqcg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2etmuqdxk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2rxptwtln.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2lesbgskn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2rdfylcwp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2evfkauxq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2apnyqcsj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2clmqlbqc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2nmwfvxxc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2dcnznflm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ktpboemq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tnfirxkd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2awtbdwky.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jiilnfum.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2aaclztlj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mwquoegf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mblfzmct.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2kolndtab.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2coaidfgt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2mhtyrkmt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2rfyedulr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wdbjhkzc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fxhvfspg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2nwxnonsb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2viagjfcy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ogwjlxop.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2epuycfvl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2sjjsuciw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2bqehnusn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ahezjpub.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ucqodsta.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kfehpnox.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bhybdwcr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hwuahqbx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hrwskbzh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bqxyiqck.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kfdwtawh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jqzhlkxz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gskpvgyh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yxiotgpt.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xbuokjrv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2gsalabxq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ucbbofpu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2sfmofbyb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2giqnrqut.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2alttbfet.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xpkosfok.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vxoomrmw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zxpakcff.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qaenyuga.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2xhdnlxqj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2dmvzxvvt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ncgwjthh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2kouumifn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tsqtfgro.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2moimqchu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ybyeglxc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2wzxhmajj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ocmnjhne.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2udjafxbp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kukykvzg.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2viquudep.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2hxcryjqf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2tqkerugq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2bqmjntns.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ctjdcazk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2xcefholc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2umtoiefo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2nmzrilwq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2csanqpqw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2fuhxzrbm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2svemxtyp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2yscwypnr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2khrwevlq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2hblwheod.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2scpfkwji.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2imccxklh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2xwiqygwi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ehunsapv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ctdhjrmb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2fgycyusz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2peuoncbs.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fwipltlx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ucpzjmgn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2unqhnmpx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dkmiqejx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2bbqvvmqo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2asrkcnku.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2cvvguzxf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2uohtqtrc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2raqfkufq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2gkimomiq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2tcdzpnaf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vvbaqfnb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xexfilpn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2stbvzsdg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cmzyiltp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2afaiezbj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2phftmvmn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ptfelktn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zhypfbzd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ilkskrpa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2uyefgncs.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2cmnjodug.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2fofdqbay.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lxdcndix.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2rpmpsapk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2djdpyqqq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2mkizvevb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vmyzwrts.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fxnwrvpp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jkuezava.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hkafgmxu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tkpqysgw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nabqjlva.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2klqoyjbz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2nkzvxlll.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2wkwkmzcc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2itacbfye.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rvecigtq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pohkalfz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zcxgkqje.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dgaqmcwa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2etzojelz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2tgxugjdp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2bhspjkpv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2qksibwmg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2syzydclp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ubowjbth.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qjduqywp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2urpbmxuv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oucwodzg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2vvxguzzn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2efggmtoy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2btkxgcba.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2bqvktlua.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2hrkknsux.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vpkbvgny.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vroqlrli.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ewhatiqt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qmepsfsw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2beejbaeq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tsugpkzp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nhhnfqsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axfzsijr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2brrefjlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tjitxags.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nghedwxt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2uvrdgrtd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ymxcmjtp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xtqmapkv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sqfzqiit.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2yukrsuap.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2uizinhbm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2flrayjam.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zcojhugr.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2equdnvvb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vdtjuwzi.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2rpwssluz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2unqfylem.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2okogprlf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uqqhhjla.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ibwwwssm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2mthyelvu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2tndfoufo.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2igmsbyaz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2talxmoyd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vkcxmewz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wlarhhxz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nmbztgkx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2affigkvi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xqxeuvju.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2nbtvgohr.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eajiqbqj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2byulinuk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2sztclyzq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2bbgkliae.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2unvtjsag.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bsxbayco.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kvmipbbv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2kbiabcso.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fupsdvla.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dowbyyti.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2dvnznlkt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xbnsrqrc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ijiiphxy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nlvmxime.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rjweuqie.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gvlthvyc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2xnlfpdfc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2luiayczs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2muphldgt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2shknogik.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uqyelsxi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jztpndwj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dfpovwza.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ggpkfzum.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2phpxgubn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2woktkcsu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vfwfauwn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2menzpfpu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2drpcwmvm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2jbmkantv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lebsfwpu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2nkbfrmuo.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2budnewrd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2tlfylshw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2cdyoxuga.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2uzrogsuk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2vmzcdnoi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ndwxflbp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2czbccijs.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2rhmjpunb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ujlpqrgr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ljbtkunf.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kprgphqv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2yxnpxest.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ysjmlijg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kwcjyvex.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2kdymrqrc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2iadbnjmz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2pycjexxp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cvyekseq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ugkptegb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xoyrnuqx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2octaphku.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2viqaspcy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2oipybitc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2veibreyz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ltrdnudy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2tyynlvsg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vhdiuzzs.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ihjkftxq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lsmkcchz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bpidjsby.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2itdvmujt.html


<!-- 参考信息 -->