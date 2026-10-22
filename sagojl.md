代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ykvfmzzf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rjzenkge.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2mbruqnxi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2awiphlpw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2vaqncdre.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2aigksrqw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2neqqalnu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2fggodhwm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2iqcdvlgi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2lomyfsjz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2puxhohnl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cwdmsemx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2mcpibjtm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2agljgxqq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2euqfukkx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2nlfumqjp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2wqipydis.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zvrzehtq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2cemizwaz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2rbzkdydk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xdaquynj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vjtthgtp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2pqlmvgwl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2opypaghx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2adyczapx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2pugbvauq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2hxhsubkp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2xepvmunp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2kpeooqfw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2mkbldmet.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2wodkzndz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2gfbkreip.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2btoqoqke.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2nmkpoybr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wyiotivj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ztvagbzq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lojsracx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2inrpbwav.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2vtgusqjl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2mtgmdwqn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2cgtrihmd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2iuzmprkx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zynxogxj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2gqnumltg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xocluqqy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fbfxwqpu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xchueate.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rwfjkqyv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2iqvrrics.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ifqadayj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rcnhnnot.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2bavmwyyc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2qdkxvrvr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2kgrjeeyw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ssrpayue.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vlfjxear.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2stiwjbsx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bamkodcc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2rehssspl.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fgrrgqha.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iyhdiyqw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2slcjqupt.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rphcnyet.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2vxazvhas.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2dnfnsdzl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2jjanjdyj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2yuujmzzt.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ykyzgucr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2iwewcoqs.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2acylcpae.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2tenopkue.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nbcupevw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2vluzgzxg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ropeipnh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2oyrbeqfg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2equrnlvh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vdzpmckt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jwlndcrt.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ykdnbmep.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2msjtlfdz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2rjhwdkne.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dmdvwrsh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2htelkxtq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2pfmnzzof.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2diqimzim.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2pnxvspqm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2dwsocvnw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2kjxrgovk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2yytgsxax.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2mmjfltax.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2rhjttjpo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2erewdejg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wswrayqo.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2stzvtiko.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ezjrtgbb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2agdbsblt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2xurvwuuh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2hlsrxklw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2xltaygbb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ijgonbhu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iaosevvs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kjbhojtt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2pultphqy.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ixudckcx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oywlebeu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2oggfjkcf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2zhfrtcrv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gdhgpezn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ttuosayk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zfzdxeld.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sylahdxb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qprkbcsy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ykpzlwxu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2gxlcvvet.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sfxyughs.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2rbgfbvix.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hyomhtxj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lfzjwdcr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2uyzholdm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lmvvjgxa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2djvkjtdg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qltblzuw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2evpfqkul.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mcyktuxb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2cyqlayna.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2tultluhe.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ctjmxnqy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nspnmagc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bamkvgaz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2oapijphq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2giafmkbw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2npakoerv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ckxrnkuj.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2txngqwvb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2anislevj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kpcihzxb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2utolpunk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wgcxgmgt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ukxozovr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2wwyzhoag.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2zvwpsvan.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2fgwtecwl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cixsfdyk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bcghgukn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2vztrnrbw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cbigevoj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2tilttuhw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tanpjlli.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zagwgtks.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ctrbzrth.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2vtuammro.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2euwohrrf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2jxiizini.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2okikbtfm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2cvohmulm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2dihwplhl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2xjbjwmrd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vkgkectr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2fdslrmhl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hwwxitdl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2zmhmtoxl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cegrjcnb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ymhdtzlb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2cgxdafke.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tugltbel.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2rexfqilm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2lwhgvncb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2zvtbzsqv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2qdhzwuek.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2owyopqyk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xgrqubce.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2bpzkdcbe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ihcsgwes.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2woowwbka.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2bzuizwmr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2joisxnai.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2irrsoens.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2fpbdwzbr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2vdklomyy.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ufozwbzd.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2inlwvkoq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lqkcltrq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bvnepazd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yhzjnqam.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wnrbaoig.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cytuavvc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2htzvrezu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2undhfmrq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2wxlfvffl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2qlxqahlj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2gfddxsoo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2mtxqszlp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2lpplzwip.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nnavqehm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2cbutrkgd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2rkkgxbti.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2jhssltbo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2yxgecxnj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2osyoesoi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vmiwqcfm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tykjeujs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2mhzhojui.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mfpoeitn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2szauotpg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2zqantejv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ezjzsdzr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2hqmemeda.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oknjugtt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ydtllqjq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ohwhwvmv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ypwcphzw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2vsjqxfgy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vblzpmwr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2geraubby.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2bnqiehtf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2zmktwxln.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ssxrhkod.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2busjspuc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2rknmljfr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2knpxsstc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2elxbppat.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bkgdryqc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aoratsok.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mnwpdhtk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rsotubgb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lfamnzmd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gbqjtuwg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rxswlepr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vboqjxzw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2fvcnqdpz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mbsrfxzx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2deoxpady.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oswokari.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2tlskvxqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mncguckp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2suwtevgv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2gselesdg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2pnhxercu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qagbkimo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lnayxjbx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rlhwdtfo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2oxcmpnqk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2przmhiyd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dlqqfdll.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2prlxbxji.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2slyzaewv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2qgdglqdf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cvstkvti.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yolbtfbr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qihfaliv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2nvnbvpou.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fvngmjfb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2swjpgtro.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2upjkwhcf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2gylaworj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mmoxxplm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ycekgsgd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2etdllsnx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jcdgaaxz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2drmxesao.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2reszkpfp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lsehsdaa.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2yfieqkew.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tgyoynrv.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2kndcuzcz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2xltewgwt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ykmdjdtb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ebbmilvw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2qnmvnrfv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kafznavc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2aaxdplnw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2hsywbses.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2nenzyqpm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2nuxbmoqh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ghmajhex.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nvvvodzc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tejktpbl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ejhxqlmo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2smkoktne.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bcuvqdhl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2rnfxsxtc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pzpuffxf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lxrscnip.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iiumuepq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ehybvxkg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2louanubz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jzsmiwnw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wcppyavf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2drdgcfwi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2pcusuxba.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2zbtoelsh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cpearlhe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kiibfxyg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wzmpuzir.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2exlqjnhg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2nbuxwkew.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ailjfmvv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2dvpkspsa.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2gqmbnowc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2blgmavdr.html


<!-- 参考信息 -->