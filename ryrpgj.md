代发 wailian999

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kqzdptii.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2yxhoorav.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2vepekhaq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2drcordfz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2mnkkqlfi.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xhvnvqtj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2pwxgqtob.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2andpugbn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ahmxfzvt.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kveojcml.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2yqkazknr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2efthwjtl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2oucrhhuw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wqyulnxp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gjwmvebc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2foxzbibu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ndhcvjms.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uexsuqkv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lbnmqdqb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2rzjfzvvv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pmqzqhyx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2djhcbdco.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2yxxyqwhz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uqtcbdmz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lucygwdt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lwbxpzpa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2bjjbirtu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2culsavxp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cylkxzfi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lhptbuep.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ofzvlgxy.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dewybjfk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gspfzlcj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wrdfekhr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nxbciwla.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2eabuqypj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2xypcrvdb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ubunjscx.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ebpupzwa.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2umdfxneb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2xpisnlnn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2mbseqwbt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kesrslnp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uqqcqdml.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fqkqsedw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lnrtuyna.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2idlvovrc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zvpesnpf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2omgfowzs.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2pdtdupco.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2okgxylvy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2wvgmoanm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2zvuvmopp.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2kpigjcrm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ixdzkhvu.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2loypoelz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mgjaybsp.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gmxitbhj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2cqrfizxb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lvehcupf.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sijyewkg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2mgtbprey.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2rpywazhp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2jiblhvcx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2oasnpknd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jozrqcnh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ymcrmetr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2klrnkvse.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wyuhkpok.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yhnsbjtv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2idbfsybi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2elgjyjtb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2sbeqzfxw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2apguhlco.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2csdmvkss.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2zwjkunbl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2nqlvynif.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2eizcekte.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2penvowyv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2sbmwiynn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2qbqkabor.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2czjbzpls.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2eivqjhgf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2eycnhrjy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2yttulxbp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2sqgpuioq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hupntqnr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2largfvxx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2noptrxnh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2laljbkaz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2bljgmtuh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dmofcjjt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2hsjlswod.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2fsfuftzj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2hmkdjmxh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2afahgdzq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ddkdiebu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lkpfkepp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rcajscjf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2tpztjmgm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xpqqyxdx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2gruzhiss.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rmjwsadg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2xdnzzzhc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2dclhndsk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lckattoo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kjyzijlh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2egummvgv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2magewzny.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yhwdwbjh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gzvrwjgx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zoqouybj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vcllqhfr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nsmvezej.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2czedccku.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lxtohksq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2unxlkspd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2oetxuczz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2nhslubpe.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2owaurlnm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lqldlhzb.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2tymdrxqb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2odbnncfi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cugwwdov.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2klgvglai.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xyedhfln.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2iejigtvs.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2nszzpxbp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2lguirmyz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2pzvoxaab.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2stlwsyew.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2efcwbttl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2thcvbhrg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uolteudw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tasmapfv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2imeklcqd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2grvdkkzd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2wfxieuxm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2sntserqa.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2schorsvv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2meaiyikn.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ncphrmko.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2tokqfxmt.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2udvblawy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oxlwwzog.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2typiyoll.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2iloztmqy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kpgfdskp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2fmsqkakd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fnhzorka.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2pfzsqunv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2mfxoimii.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hmguwcso.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2lczhumtv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2rktevfos.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2lyonhowk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2yjlqnzxe.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mebegglp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2eplguson.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2deayfhcg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2oxvpybjy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xovbzgon.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2dhwprteg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2gbnhvsus.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2hyjwmcjd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2yrokkbbw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2uitfdkxw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kmkyvpaj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lfvomqey.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjnrupzt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yzznqhee.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zbabyigl.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ygieepen.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ijfxqurm.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vsyflxtf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2gqjirhul.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eljmrjqw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2xkqjkkzz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2dexuzyof.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ktuqyskk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gmidvrmw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2agozadfx.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2upousmqb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2kkptnsjc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2fhlyaelh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2vswbqsnl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2cypoosnj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uudtkabw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ehldnwde.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2dmsfqztv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pspbwoza.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2dqneeiaw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2rnnfmxzp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xlqtjpff.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tgwbirpy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2nrzszrmo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvcxivln.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yoewlaft.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hsetamdm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2vtykyeas.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2qngnjzoj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2qdebynen.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hxoeyyiu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2kbewateh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dpawqmce.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lisuhegi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2cptawteq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2duzxjajq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2yynhbqoh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yxptavxj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wbddbchx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2pbwqsyxi.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2zfqzdpfa.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nciflvra.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qbnvpgyw.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sykvjevo.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2klickiik.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nhdphxht.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wugkporq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2txvqiqto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjrgqosy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2dmkkprso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rnldcnef.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mxchszul.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2obfmrtce.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2pvkaylms.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ipbttyrz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zbtixfqr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2mkopirvi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2npcorido.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2fuulmnrn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rpgwcthl.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2gveqpxsh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2agnqgjdp.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oxdqkwya.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mlcimyfk.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yqvjemke.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vrcstcei.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2pzkwofak.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2binubavr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2gzdsnlzl.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2uofwficp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ibcvvpvp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2omfscump.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mfycqych.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ajcjlcut.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ksadduml.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2msbkiuod.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jvktincc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qqqgsxjn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2fvfuoago.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ydsdzmzc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2rjcocdbr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ynidhsye.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hnrusxjj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2napbsqtb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2snwgmwlt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2oftvyosl.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jxvlxlxk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2jnnsgzvv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ytdtxaoj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2irmcahvw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2accieeeg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wdmccdnc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fjdkfmxg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2bcwexhvn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sqolhfmh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zniyhrsn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2znhrjrow.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kuoxzwer.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2bsppcmqi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qswhkyns.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2frurlstg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hpfwfzdn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nvdfmgub.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2inkniffi.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zywgnttt.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bpvscgri.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2avxtffor.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vjhduwtm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vpednemm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zfpqzpcq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ycvwffgp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2hdfmfwdy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2sginkgdc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2kepaporq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2itiiubtj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2qiehfgvb.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2sofdoqhy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jycgsfuh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ejzgrfen.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2emykcoqv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2psmphiez.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bbwpjrdc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gzyxegzx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2yowzrltw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2wevdlewj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gplpkjcp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2seuybnyz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bfjwbfjm.html


<!-- 参考信息 -->