代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ilutbxnq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ezfycqlq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2veojmtqf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ttqquaks.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hmrwigcp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uiuqlfir.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2dpvrjktk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2wcoxgbgv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yjrnccjf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mozfyfcl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2lmfrbfet.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ogpkgmuz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2dadsoplr.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qsoaapqc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2giyivcae.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2sgowwtwr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rqqagvrd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2aurdsqmf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ccwydoio.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gmydxsuu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kgvfzqrm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hrnaldqp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2xisbckoc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2jnqfgmly.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2avatttst.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lvxkkqyf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2iiputtei.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2htsfxoxs.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xsuxjyif.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ogiongey.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cqhuclcy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ywtplpwt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2xrpslmdu.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rnyodkcf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zdqsgojk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2iaqjidhc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2bsdwrgsw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2poquvhsd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mhyaeqbg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zrfhgkrf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2osdoxhki.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tvpprnoy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2hcvytegw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2lznjwzve.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ofynlikn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2zxbfenfu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iyrdkgnc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2nlllffpe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2huqdpyzx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2nrjqbcgy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2gknsvwlb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2sveetgia.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2fcbfrzzj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qqqaomsc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2qoacxhoe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2myxckvog.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ggztebaz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2kquvcdaw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2elitaxae.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2nzkfxazb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2akxvgdsm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2welvkuph.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2lxoeyrmv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2jrzfvgmt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gqkyzspp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2psumuqlo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xlzxamoj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gpywrkjv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2tjatmoxx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2jiruxknp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2whxhouby.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2uxqilowu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jpoxkxea.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2wzvnilpd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bzkdohyw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ofcinxlc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ptckjyjp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fqhpembd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nbesrluh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rcnwtqie.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2zhdsqytj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2yivhtzua.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2iojvenhf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fpmujzri.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ttndwrte.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2sxnhdroi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2rfvnjgsh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mgagonsh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tvpzvmac.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2txoubhfo.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ykkgzyqn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cqftevyc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2gdhuirfd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2sbqqplyw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jbmyvyxc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2buuvhmxw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2wyhbxxtm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2rcqegcsy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2etfdbbhf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ezyyyont.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2jcjzfuce.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cvtpwqim.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2omkjzaax.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vwyxqnwr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2xsyqfcbw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ggzmmoky.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vlocpquu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vmpwopwp.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2qfqlniux.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zxmrlmwl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ocmqngle.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2esyvflic.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ebtnsgpl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2mmrsvsim.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2bwbzhsyv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ifjsvqcz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xpggepwx.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2juqbumfr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ynpyityp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2suucaemw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vhtodbai.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2zbzxgcan.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2faorwuun.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2qbfhhnvt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2cgvxogjr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2pijhjdch.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lovphxri.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fhcslmsl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2zfidkadv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zgimmizd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oxdxwufg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2isdvqort.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fydsxctf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2evnguirn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2codgvcak.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2vttxzxpw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2jndnsnkf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2djhggabe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2jttrbknn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ktutexru.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2xyljuxgg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ralveoti.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2gcyoleut.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xkjaacar.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2dwjocaie.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pusyjikk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2xyllhvna.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2lkujcezg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hrteagkm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ylxrhloo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2eralcime.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2yfrnjuuj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2wqrskhru.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nwhpdbsb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zkmwszzk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cowcwlux.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wohdloyt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qgvtoxmo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2dlvkdgrh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ahbziggw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2tdhjeqfr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2wpxezfia.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2itvxbngb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ykxnfrfd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hlyydlpz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qhmdiilj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2broseael.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lruvmals.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yibfudkc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qiugqrxn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ozzcqzwm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2twhijqbg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2espiatsj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2aohckxtg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2muuqmvuo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2lciofjer.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2shllgewx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2odrklcfx.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2bipkotvr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2erqistts.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2rpvrwvty.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2daizybfp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rtuhjmle.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2siexcryw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qkxzvufv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2olfdlrrb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2axhyavsd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2uwrxfljv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2tdfpouex.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2drwwufsy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2zijkadzg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kcgctalm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uyuzkidf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kbhuvecz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2wqnnrgqb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2bbvrnjnq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ckcbgzsm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2mjfrhnrd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2kbxdnsby.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2sdwruibx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2lwuffzge.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2rlkmzxrk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2cahmukgy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ghgfluow.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2inspzdha.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2gcsnrlmz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bjdrtfrf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2smzgwoss.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2fbdhncsw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2aftojlkg.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sfsemqjx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sjzgvoyd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2liuuheej.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ukleujmo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ksiwfeql.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2odziccel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2taorclyl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2fjgmegsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpoiylxq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gkuhatmy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2kegavscc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2zbfwwjyp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tlhxnzqj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2whsojsqs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2xeoomyhz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2dtwdzazk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2cuqsduua.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2axiqpwlb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2wrfghyee.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hascklhj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tyqdbewc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lvslkwzp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uniupcga.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wlxfoqsv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2wipexeqk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hhanqynj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2arfgyzoi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2picgirvq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2clnkjavb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xnyifgpf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fbsxssrj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hrqamgtc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lbockdhb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2evgbnnyx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2snygjuya.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2dfwwdmgk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2gsgzghkp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ukfbvbyg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2gjmdfkqb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2algpgkqw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iyvpmswk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mvhpxklj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2riujztqd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eackzfsf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mxkjeuww.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2rdfhtoeb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2entxdulk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jkixtgkq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ajpbrucn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ghloexki.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uqykpkcj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2wmhhowtc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cntiirxy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2klcvbndu.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2edcnhhih.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bgqahocp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ylxiygke.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fwpqnpkw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jjtapgdd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bklppqwm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jgnstayd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fxwezdsm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jrvckswt.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2sbcaxwsr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2suhprlgd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qxjanjte.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2hauurvcx.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pxaxlgok.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2axngubri.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2kdrmphmy.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2xdhjwjrq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2jorwpzew.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2tpxaligm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2glyawngu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2pdkqdchu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2afuvdion.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2sfztkduu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2sfubiuzr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2osocpirt.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qibjnajy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2llgkmzqu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2hfsmtztr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2uydavngg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2agfnwpkx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bktjbvgq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fxxkysfi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2uorfvxvv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ilakdoya.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rfppnwum.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2oydsdwkf.html


<!-- 参考信息 -->