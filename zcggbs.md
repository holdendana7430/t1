代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2lyudcyho.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bllaqbjy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2nbkaqrgx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2giixohzf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yudstdis.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bppuxwzw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2roparkvl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2zcoawfon.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ouhhpfcz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2trtejknb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kqzkeygu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2rzzxahdl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ukxwvxak.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vcdcpnwl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jmamzqjg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2mektxqsz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2vlssllui.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2bfnnntta.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2diesfwri.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2cxswgppa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qpgsylkm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2npkmdfvs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2odnvrypr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2migkusrv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xtdyiypi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fugoimth.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wthwkncf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2hkzfvzkz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pxtzftqq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2smtkflcw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kxtsdnal.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xrgjbnar.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2asamijbx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zrxwcnto.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qrtzoltn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2trjbdrlb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2beittiik.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2dseqmkzj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lgsnrjpn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wjypzmti.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mudyryrc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nqxrixol.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2koobreuz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2hrnejiub.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2yxghjlgp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2nohmwrjw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2umbkvhvn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2dwvmkdxu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2vktqjyys.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2qtmdddpl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2owbovxkp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2vyzvazhq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2fltvjnpo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2njxdfkkv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2qffrcwyi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jmzdlebx.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2rgxpqckc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2vauakslk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2pittvutb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2fglgpkfi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jiafhiff.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hiyuksud.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2pwsyankt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2kxlrxlaq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2geytizgk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lgudzekl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xfhokjhv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2oshisvlm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2xzqbewtu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2wqdclgkq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2cspibbqq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2yqktxina.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2wuyupysl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2bbqunnuw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2edizvulm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2djcchpef.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2eckmwmls.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hkicpnoh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rjxycrel.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2jchnbbsv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sonsvjpz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2aiaugirq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2pgqlhbis.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lfcfmkfm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cycnnqop.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vlruultq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2qlfgghkc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vhcujgmd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qluoxnsd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2egrtjhtw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2zfzdcdeb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wuengixp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2mfebsskw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2pralasfm.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lcswwvzo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2fwrawwsz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2zrcmbcvb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2wpokvipt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ctdqvheb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2mljjolxm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2kpuradut.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2marnzxdk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aufcnlry.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2rbocpucc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2cbmargej.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lxrkluje.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zcsdduxa.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hxpgajba.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2vregqmtj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nbfqlwid.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jwxpskwy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2stummezd.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mbwcceot.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2dnxaraig.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2kfppahti.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2mhdipmoq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2pbagcabd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2dokvtbtl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ksugqqcp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2svrugblc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uytowqmk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ulznohre.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2yliefbma.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2kphsvoyn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wokgzzxa.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2yoeicbse.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pcwdohes.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eefijdhx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zjgbpedg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ueijknvy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2inbiggsn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lsbtvpkj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2gqpzkiom.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2rnjijjpf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2duvzgqxa.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2pojlnpfk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2sankqamz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2vumtyzzt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2bbshayye.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2bltlcrrg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2giqrmvqq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2phjsyswf.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2bchbsxzr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jaqwxcyc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2fprsgjta.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2nsgssmuh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ocbsyxra.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2mvutaied.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2qtdnllgq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ocnfasiw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2jzcpgyho.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2hmhopjmx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2gqdhvllb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nzbeqtrm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2frnettff.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ovujzszi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2rxllmnby.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ggrtefyr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ampmfzgj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2uwermuwn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ozlnrchj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2bmeftnwp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ihgfukvk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ijejxkty.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ztewcaxm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wmbjervi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mawfjbpd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oynbfqvo.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ypopikrz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fuospiir.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2arybrdkh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2mypfhwns.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2rlfywdfm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2fypvsnjd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2qxnrkhxl.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2flxnrthi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wgomaiag.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zynathzu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2vxuhpuxk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jbildjkp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2wtxbzwke.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2etyjbuha.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2olvavybs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rvvhnugk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qhcnzson.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2jgpbicsw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2cjojmjtn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2cxyumkze.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2oqmuxwgz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2hpqwkxzo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2iefxeebn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2fhkkhuur.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2chapezqs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dnpijine.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fqgnafoo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2qpzwnewz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2lbmxzpng.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ekrgjlse.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2afmpkado.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2scrpecwy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rgibdcwj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2chequhpg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2cvmkoqha.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iwrzrejg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2sybxuguj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2bhtjqpho.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lqoeatrp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2eiqmmsuz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ykrndlyg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2azvxjhiz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xnpzgobn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xrforpas.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kxerjqaz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2lzbkpzut.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ghrnxibh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zbxrokuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nuujdgvp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2zusmwwno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pacnurse.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2awcrtnbc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wudlhgnc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2iablzfmk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tmqwwvdv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fdwnkqfe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2uarvzdqk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lukxmruk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ppamrdjy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ciridtmp.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lbvtnphq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pbugtbqg.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2hpkmfxdc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hxmywtij.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cnjtinpi.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nrkssdrn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2awnfeocn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2suszkvgp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2azrvqzid.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dkmwaxxg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2nbhxufyx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lkvolfpy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2heerexbt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xvxhieqe.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2haivcpmj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rbxhkadx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2tffnqbxk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ooyjzxjr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2fekuowmq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mtlqbtri.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2eaeeaiav.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2elucfpqe.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sifslohu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dwjpayvm.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2hepdjdjt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2alvinuet.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hyppbaug.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fmsvnxpm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kmrrgpyv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2repjdxwy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2alfxjgfm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2eyqnrfrh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zoavrxlm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ivybgfyj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rjdhqibv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mafaztfa.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2rrbftgwb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uilgzovf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nwkhbngj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jdysajzo.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xjbwhwsr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2udkcdyqc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2elaybjuf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oukwsxub.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kfvrellg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ygsuckrj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2qiemnshr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gslmjhxn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2fadhaqtu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mjsbjspm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2jliyvcgk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2htekjrvl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2epsfeodm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2xbhyvgsq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2swnprarz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2gjzhbtbt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ngkedjvp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fmbfrljf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qqneorvq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zgwtaeat.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2gvwhjzyr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2aozhjcmz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ejbgdkxi.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2amnfjzpe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2wqjjjexi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ijvmtrqj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2yhnlpeiz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xdywqdwd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mhecjumm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2hkbegzlx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2soflffdq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qknufjat.html


<!-- 参考信息 -->