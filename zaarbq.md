代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ztmlkhvk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qznhndof.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2mgzqvuaz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2nkssyyrd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lpyvbkaa.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bwisjrzk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jelxkfeq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2yiramihb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gghlfyda.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2saplqciq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2naqhneae.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2dssqxzcb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2wrpntsws.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lwdqtzcf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2oqremtax.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2awcfsxxt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2fkidgcsp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2mmppnnjq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ghrleaev.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2maawanbe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jxvfsgew.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dhigbvmt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2taeabthk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2kaoroovk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vhkmslsm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ecrtqoxk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zhugkhag.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wmxxmjkc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2shxbfuth.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2spwueowg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kgrgbtqr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nrtzrjta.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2zgfqgfll.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qjuvzcvb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2dtmwglde.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2mrmcosjj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2duyqxvdn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xxtoswae.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yyamubjl.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qqlhglml.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bjxplqaw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pkazsvri.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2hhpsbyep.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ubdbivwq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gupxrpek.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2szycumof.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2stxzhmsf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2flvfpwof.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ofhhygbn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2hpryqrie.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2obuxlsst.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qedfohcg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fdxjzsdt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tddcszjm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ecibhzfe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vxjtmest.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2pumjbpof.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2wivxuwsq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2mlmfxgqa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2nkxtbhdu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uewrqopb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2smtjczto.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2rimmsvke.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ftqvoovl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yeseayun.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2oizhhbiq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mzfwjmsg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2shmsptzp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2iunntddp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2wvwlfagu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2devqtkzo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ucukvfrz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2gllaqhzu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2evviokvo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2cszcejac.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2vnzoghks.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2bwgtidam.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2plyxdiwv.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2yuhutfql.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vyltsbps.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2huzynqaf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2sujcggqw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ozocobmk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wyaspuxq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fdlfgavp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bdzfzhdx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2jwcjqqkh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tpdorxab.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2aaoktclx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2yjkczcla.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ppbobawr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2pyclauzl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2qqcfxrli.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hrvzthbv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jtonqltr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2jmypztfk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2btvbooyb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2hiatrwry.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sytswhmt.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2zmagpeuz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2doifupjq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yyvnpprw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ymeonruz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2munazbdi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2upawjnqy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2pbssoyak.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pcsgcrrw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2adfdgdlg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kjeedpxj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mpihclbc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2tuwjoxii.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zldtxtta.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gekaadpa.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2wljggkrh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2xfcllgrm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ydizecis.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wecbyxnz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2zwibsuun.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rcmrkshe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ywwdvviy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zhusjbgk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wlwzrdsb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2kpkxdpnm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2fxawdqnh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hjsvneud.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2pnebdmcj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qxzfzsgr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2edzxyemn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2orfuxpsh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ssvckymx.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nujqdvvn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hmquxosx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ulsttsoy.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2yrrlbwgk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2rmivcaua.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2pscirxwv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2tbonzqgy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ugudbcqf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2xnquefqv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2hmcblgkx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2oiwijrkc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ydypoafg.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ehyyygls.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ujskcnel.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2enhcuwcb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2clsotsmr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2yawjkcun.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2oaqlnrur.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zvdougko.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2tnhomfqe.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2yxtfhdjn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2evmctiee.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ixpqknlc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jwydhfte.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ycuvvvra.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2fyucerjx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2thfeyuey.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2akgldaim.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2cauhmwna.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2rmlawicw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2kuhjmxve.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2gceqtkwk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2aywhvffu.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2speacrpl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2opwnnzmu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mfujtapi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mcsokhem.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fishjstt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hcudvvff.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrwaoxgi.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mswhdseg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2fbjtvpxc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wxxkqtti.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2krqixrws.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2fnsivkcc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2imysdnvy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bciwunge.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rbqdmhsg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2sqiyehdm.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2peqwfyve.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2iirbkxrt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ckjylnnp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bvthsach.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fbtblofj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rhmyldby.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2hyjwnbys.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2myymwyhu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2lhxstglo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2bxmseycs.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2stgglllw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2revuvmkn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2dhofbpqg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2lsoufyeq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2esucthzh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hioxivxy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2snwyldbx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2qbqflddn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2rmqbndtq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2gbjytbwk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2yutebubj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2dhthpncn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ltukcsrf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2dertvpsv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fiyqxobm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2nlkgbnry.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xwdbcrvf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gwxszwbz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2kyuixutf.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yccbxjwi.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bzbotkin.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2stxqhcnl.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2spqhgphf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zllylpek.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pxpplnbk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ztixonnv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2naqnmyoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bssrkhnt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2nhmbonpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2octgxjzm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2idnykabn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2cmnhlbey.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jpylkauk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lvhrurlq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2eufabsqd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2qyyhmzbt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2hcszrjjv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2djkhbbha.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wqtaynbg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2agxnpgwz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2swspsfok.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pvlcivhh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mqbhtgjt.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kusqkmec.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zynbnogq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wpwrnklk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2kzmcbicr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2cwteifuy.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gslywgyi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2crtkaugv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2joyetzzg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pgdaztgz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2frrwaavt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sxdfpjya.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dpsdqkix.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2sjwjspza.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ikeiqdau.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2tnbxeuim.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ouuzsusa.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2lukkuvwm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2mjsqixao.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iokzceol.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lzjzumar.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2lhsdyzmq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2penpztmp.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iqojailw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2owdaiocg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kolsthge.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2yluzxjmq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dfebcddt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2obbhadri.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2thmyaiqv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2rlctqpcl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2zukuateg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gyumxayf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2fytfxmdx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2utqfolpz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2taqaoyce.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vvxoelzv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wjegckpw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xogwdsdh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aivqdarr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2neagktjr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2khafgtos.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wjqgargg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2kgtmktbh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2htitoiep.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2sbdqijyo.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nnygzvpv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2pxlkjoyv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2febfsqqu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2xihsnfns.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ynvaqwas.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2xnajspsg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2vveufiwe.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2rqgwvwrj.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ybvjedsn.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pjsrfdkt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fzyjxqau.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2behmpzws.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nbfdboeu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2sspxbdwb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2lzvlbxps.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2rsyapjsk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vbodenhq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xwgsmrzf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jxwnguwn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ybhxaebt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2iceendbo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2tctjfwtf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xqfqnsmr.html


<!-- 参考信息 -->