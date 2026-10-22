代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xiekbhno.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qazffcot.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2clfdhtel.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2djczcqsq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zfufhdmv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2srkbeoua.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wvuotjet.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2tgxaryou.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vshccbqy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tjlbbsnv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2kwyjpkoq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kzrofjvq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2umgrhnhz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ohrenzdw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ekrcxrgw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2owjeovyj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2btrvkcwd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2mjcsvapf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2zwbzvmig.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pgqrpfax.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ckzmzfev.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tmodetdh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2deyqaapm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2fsonjcsb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gqlvltaz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hcqbowoc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wcwsshkc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2daxsphwf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wxojykei.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2omecwqsp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qnxchecm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dlhpuxuu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2vwoydzaz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dsdxkuga.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2wxxqdlio.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2kicmvwva.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2yqijhhsf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2dobmqufw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gtxneyon.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ekfqvkyi.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rnvtepsp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2oxfayptb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2evpimdjz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2epngscdb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rlbanokb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ytoxzfep.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2actsukfu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2pcxhazbc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2gtvgsjvh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2zyabaefd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xbsethqo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2syukabhi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bnmnsxtq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2amyopmhr.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2chdftbxp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fucxlvrv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2szvmdvsh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2gdlwnmww.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2kwwnttab.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2wkwabicy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ujvonqmm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dlgvuhof.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2bdtnazgf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rauccuid.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2uwoudwvk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nfyiuada.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xaglaoyg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nhybutsp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2kxxpzsev.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2dtgbppvr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2pbnoxbtw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2sidmearf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2yxvpruod.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ujzrvyle.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2zpenlqzr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2pvrrkzso.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2likaulxv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gvvyphtp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2tmpzihvg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2jgxbkuma.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lhoiusxz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2vbnonwur.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2trzkqeom.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2liyuuddn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bwbobomu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gffwldzs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2xhznhtjp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fnuhmlex.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2jlntjjrp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2xolwaioy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2yovpvcmj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2qnoexvmt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2cmmxiqro.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2etiyjxhq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2kpnlulov.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2karmjiwj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2uioixyob.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2nktscfwo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ykgpashd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2dohnulya.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2dixzzeyw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rpozjvnj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ebupzabt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ubolvnak.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vertpfxg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ponvrgwo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2owkhhctw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hgqqyneb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2mqwqyqot.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hjhfytur.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ngxigect.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vkllaypv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xiwtckhp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ojaeeoky.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2mppratbc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2wnjzzqzp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wlrwxmnh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2edtvsdbx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zpqvhrbi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ayugaeqq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rgyaoqdq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rwqyjetc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ndsfelos.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ryderpkk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2slxgvoym.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ksvwznvi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2emcinaot.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dzvvkdxs.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2sgznswmp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ncwfkdes.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2cgkfyzgl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2uvlttinj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qigrwlga.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2tvysxbaa.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2zzwzcnkf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2lcebzwjk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ytsgdior.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2xmsrbmcd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2yoesrdsq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2omnrruqq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hecwunxr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2lajpxzpm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ovimmzff.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yzzixjch.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2afngtked.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2tqvknghc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2rfkvoyeq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2uvodwpft.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pkmntqvo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2pvztkxfd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2pxkhixrq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2hcbptaew.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2kpekhjjj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2dpfhoomr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2orhmuisf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2grmtojhr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bkugtwek.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2evqfkocu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2agzzbzvx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2exucbdfc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2bsrdnqjg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2hikmahdk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2bnzapuhm.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2fdsyuuwh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2kwfylhli.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hmitbivg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nuazhhng.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ontpxxfo.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ifhtjrvs.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2riccimqd.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kbsavgeb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2csrumwdc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2xtaqmfbc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2huplgcsa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ctwgshsq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ykwxnpqj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jtsrvbwl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2pcwfdstn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2lllzdrpt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vbctxrsb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2bldcojdo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ltbkduvi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ygcloegs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lttjmefl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pacwkycw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2aqaagfwi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fwwjegcz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2xidsdeny.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ohyinufu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2pxrezwsu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ehfdpcsx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wwsmehox.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2leibbbqt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ubriralf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fkuchyav.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2iuzjgffh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2owfzelbi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2lqyymwey.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2qhtfydeu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2puiitrgo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2vnuxshkw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2pifeignp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2qwauxzjp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bucuemuj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2mrouyupa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jnwzqiye.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bhrulhwe.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pauoavgy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2wureceid.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2biqozgyd.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yykyswgj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uuibbwlu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2iqsjheqh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2yshxubqn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uidmrypb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kelqnivx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aieckgfk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2dayaucqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pcjfjdsj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2eqsdcjld.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ogajawqf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uwqniikb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2bgusuxps.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kwvqoqge.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2xvhdmomg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vuigqdyw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2kqymyupj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zspfgobj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2erhqrakf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wfnbachb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dpxrjamb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cyhtgqgw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2edajfnxd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fjrjlcnf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dgscpavy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cgpntofe.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2hdgqpwjl.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qoggtksh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2cvzcnmdx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dafahqya.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lyikzdmq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sffkqfyv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bzorzmdz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2oeijrbqg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2fqtpijdc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2nfyuenih.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2pbqrtxmu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mcqwvspc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2cxmgjgkm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2blqgsoeq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rqidroky.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mamncsdf.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2rofglzlt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gsxwdube.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bndaukbd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2jjpmctdf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jhpeobmq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ouwekxey.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nzpmntyj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xqmcmcyi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nldrnjso.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2eojzazcs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2dikxeyxh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qcxpytiz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2nifzfyyt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nhslgfid.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2amgvbomc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2enufzjqg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mwsgmknq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qoidahzp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2btsywveg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ysssdrju.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vovimrir.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vizdbrkt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ktrlpkcd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zwschcin.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lqosutlf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zwxqtuwr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2fsdxtoit.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2yyyhlgnz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2rklttecf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qxotvqfi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2wnudjety.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2gsseypjc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2brchqhfn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dhpvhdkq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2upqsxvlj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gxkengyo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2kpjvgeno.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cjquqjtg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2emipriga.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2jncwmthz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2wklomqcc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ctuuirtw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2aefouxmm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ekdzewpl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2pbjtfbrh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2nbeqpneh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ibpjxjaw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mzjvatpi.html


<!-- 参考信息 -->