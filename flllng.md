代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2zvlrqbhw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ryungqgj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2szvxrdgk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2sercxlqk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2wxxkyvyi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2knytfaxn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2vguaiwbb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lhgtslwg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2vzssslpx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jdnyigsh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2hvdlkgxn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2mwssblgd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2exeqwxgf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ufgaymjr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zvuwgcdk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2zzpibmex.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vrpafxxm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ltguiyun.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uqjtnbah.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2mmfqkqvn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2erngzvez.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yruzhjwv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lzvjgnpx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2qwqmcyax.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2baowbwsa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2yxqygoup.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2bnbhopno.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hyyboamz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2uydpmtqe.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wcdzfpzk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2bhxclzaq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2vecxtirk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2uyvjmbry.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zjgjtikp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vajwvrns.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vxoayeqq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bmtxydki.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xhpwlniz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rnnrkvht.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2yjapnudh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2bitcfcvo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2raweygjb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2hjhbrmbi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2qtuxeqzz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2umlrvivo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2dgzrfbyq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vjdxphqv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bqhpwgsy.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gvimtrsx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2effhpgib.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2lwabfxyz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2zucxdamj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ymvcqfnf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2yibeekup.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ccqoensf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ggbmreev.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ovrnmyjd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2axbdfoar.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2dafwlotj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ulgcrbej.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2kvpuipaj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kqooxbil.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2terzldqh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zcteeseb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qmjfmckc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2aluudbze.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ubeowsmz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ldzvrfty.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gbnftomw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ragubekt.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2uhgwibzq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ptmuwqhr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2mtavpbsl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pbakghsn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lrlfdtat.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wclkvuan.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2sazjboyd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2gqxdvvdx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2qnfzrest.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2wonsdueg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2iaaazpfq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2znhbdowg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iknihjug.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2rmtltybv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2yvsptgbg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2earnrvwo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2canhqtyq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2utoejdzb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2utgcroez.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2cqnmlozx.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wsxbrekn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tpbmwtlk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jyullzjz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uhtdnqmn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2cnncjawf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nodkdwpp.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2azpxbhpd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2jfhawpxx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2visaxzkc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2wzpnquoa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tsnbzpuy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ycvlmmcs.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ajxpyhkf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tsgzwict.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2burrpajp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2awkwcxdp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2johzmlrz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2mcsvizpi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2cptepgft.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zsjfbgvr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vkcbtluz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aywbzixu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2lqbmogna.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wslnvwiz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xkeflnpk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rybmwqol.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2jwklbiot.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wucgtihp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rixwirrt.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rcfciopd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dhqxupyj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2putwdiav.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2szlkbopv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ulvobnlc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cwolticf.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ismwsdsw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2irusjqmx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ogdrkmzl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pzgdxqwv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ynbexhkk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2rfojadwg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2kakomzcp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wangmyir.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2lexbdfeq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2smiavazy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wzywfcot.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wkprutbs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lhtmzlqd.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2btlvmsvc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rxhsfjba.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vdvixpmb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2rnxzkrca.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2tmefrdxb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2usoaotzj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2wsvqnotf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2gkmachnb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jwxpryxp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2uoktpznw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2bjkpggxi.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2foermacp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2npybcizv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uqapalnt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2jpuvbqdf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2dxtbodtn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2njqmbrcp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2rfaolpnk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hrdtwmbo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2vakyovyk.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2fxvsitle.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2wwepvjho.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2nqabtjdg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hlivrjrk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2kdeyjcas.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2vanfgrkp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2twkwpprw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zyohxqli.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2oieawmdl.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2lxgyfjic.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2keepcxfj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2doqbgoyy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2zxhxrlah.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hxqcdqdc.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tpijrogg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rnnlvbzk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2teajwnuc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rfqbgdnj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ujunjnzl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2dhpjhfxz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zfvnrqay.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2hifyaswy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oucevshf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jtpurhce.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2wswsovvj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2saleysvu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2pmymwhmz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2dvbszujc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2wjgsfvhf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2kwmrxaft.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2hwstqyhp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2akbrqaeq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2hezswevk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wrqbfffo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pvehyyuu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2fttwlrvr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pxenephz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ynmrzjch.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2omutlszj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2nyllrbnx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2axxmadak.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ecpgvujf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uhzxdjqr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gleregfv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jprskgfi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2cexensio.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2yelcwzbz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2wfetrszj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ljbedbhb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2acyhyjjm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zcllyowo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mqjzfbzq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2qaxalebz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nfozdhbb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2vcducban.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2umwmddoc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ntxwbhmm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uivdpnnv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2icfxtfrf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ohogfucl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xndzlrsr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qhszqkhy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gvkhlegx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wxvorhkz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ozcodnkn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gnzgiruq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wbysmvpt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2qbeywkoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iguofubg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ujlfrhzi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2mhftcpws.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ejzdocbv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yzxxantq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aodjdtqu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ndqnqvnn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2gevkllre.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2zrilkblc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bqnjyijx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iqqixvux.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2iaxxyjgz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vukrrktu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ffwbpbhr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uytaxhah.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2duyooodu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mtzlbjjq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2stkdgzpo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2dyivttjz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2andtuwlw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ldvlnsez.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hoqkdznb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kwcsmaqn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cdigdgdm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jgbvbxsv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2nxaaptgm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bdninlci.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zdheoxqz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2hnlljswr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nnurhcvz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2piyucznu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2lfdsjido.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wibpkdzn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pkianvur.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2oovdhnxm.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yknaqhcc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2eccnvlqx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2zumzetub.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2hqrxmapa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2fradxhqg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yqsxqvjo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2vyvmglue.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nsbsydlc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2zchvyvka.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ycmffets.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ykrimuxr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2jmrogjck.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hggvuhzu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2eezsuxzm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fxawrgpm.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vodthlxp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rlrkokmn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mbgtpgjw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2badtzadq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2odcxyemm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2kapomstx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ixrkfstn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kfihaumd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rdmxxtxm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fzedsqix.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ogkdxdnu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yurisryf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2swqxvkcd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2dhorexre.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2rvnkhebs.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2fttmsdma.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ehrpjewm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mfykxtek.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wdizmiyd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uvxajdzt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2zpzlsqlg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2koimfsse.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qqjoobeu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2cdyafybv.html


<!-- 参考信息 -->