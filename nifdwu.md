代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rbmwelgd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pmzeupxk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3apgqzyub.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3kcztyzzz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tvslxhig.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mozxvodg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3qusteizd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3fkurhqmj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3qtsrwkwu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mvpkmfnn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dxkzsnru.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3rhtyzldr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3izjjfgsi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3lbcrbkti.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3jmqdcqms.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ihsztvzz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vspwrizn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3feztnzby.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3rguvobnq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3htpixpir.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dxrrayfn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jznzvhdm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3aowpvojs.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bmcufvyz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3morwaebv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dcjmguxz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fpqrsbom.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rzzxhmwp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3mhihxvsa.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eqnedsaf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dpggrdzy.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3hbqppzgv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3kmoxjrhr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3nouxubej.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bhedfpvs.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vrceemqs.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uamhifhr.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jnppqhdg.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3jexltafw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3pdsjoynp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bwcxwyeh.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3jyhyaktn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3uvxmwpua.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3xeftgfgk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3lphzfnki.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3fqatyjie.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3udnybjpp.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3jdajdscj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gqktuxdb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3htscyrag.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3jutxftur.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qratpqqt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ekplxpvv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3nysekzil.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3gvwwibza.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3yofoekly.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fhxjlpvt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jiheghmv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3bsbthwdf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ztjmfxua.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3jphzbjym.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tcmbndbz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pnlrqecf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jytulhnx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3yfefagka.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3vmjgrfqj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3owftlxgn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3rzzzanvq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3jctdewia.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mnfavfse.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ixnuncqe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3exujsamf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3rhiuejvn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gdoaihbj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3bxdxjtww.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ypsirvel.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3oookorlc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3whckejpo.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3fhkmpkvf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sagqrluk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qywbzckx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ssiejuny.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3mnbbldfm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3samnwjvq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3vsnkjyhd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3vbixlqrk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3eumaocce.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qotahajd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ftfovmdg.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3erliaqvk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3etemgoqn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cmzbgfoq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3dpyyefgv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ndicgock.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uxjncyqh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3zoiegwpl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cvpdorqs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uxyegejd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yuaauewq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xycdftgi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fdbjofkj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kfreedno.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zumgjifd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dixwhvmz.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3boqqjkch.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fcpxawuj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gzvzoynm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3expbuith.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3welhlgqp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3fezgzlwc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3rgikbykg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3tzgptnge.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3mawnegtk.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3uqjzapvv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zhofkuda.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ohwzrwfn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ximhqsns.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kdklpzbd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3almvcedm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3lxoonrst.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hnjlngdu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3bwpcgpzb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3hxrcsfzg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jwlqqtwm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ivawmmfp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3prvnciho.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xbjdbssw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3csgtkari.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3isnbqwyx.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3gigqifwy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3kipasuky.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3vkhgfkgb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3hwjzvjuw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3nbxtzdlq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3itcpescj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3rtwrlmdo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3lxkltqta.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lwvowusb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3sapakkhr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zvtjsscl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3bgyrcths.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3gzjrqjbh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3edzazajv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3hycqhhqb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ixuvbogw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3yfyazhzu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3hdiiqowk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3imxxvdnn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3pxdvybnr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ljtieeeb.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ntwlxyen.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3stgjhzho.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3aszpawib.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yagxaivw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zxfalzoh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3uqlpjqnm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3qbquucnm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3yhcagkib.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3maqmtogm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3umsrsxnk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3reguqtrr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zflfkuwf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ugzanllx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3anscenku.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwsmnxav.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hhkecwkz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bztoksqm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3tuosyyke.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wrbkatad.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3emsobqgf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3fkdsgidv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ryzhhzsc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3peezrsdz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3sulrxfbq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3kurasvgb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kxqwhwuf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jgjbsfyl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tyfmmbuw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3vvijufti.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pbruwmjk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mpioarer.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3dhdohvmi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3oiojfwiu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3nansmotf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ahsslily.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3lcmjbjrt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zzjvcvoc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tnzktbse.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3cmdwhwwi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cutxuvgt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zubznozr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3pcdgpwgw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3xmmfvxwb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3cenyqrlc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3mnhkppqv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3enrhifvg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gmxaivwd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vvqdnnup.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wjfqsjjt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ufknjili.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3mvqhtuqv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqtdrorh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mmajqvwf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3abzkdvmt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3luscflvs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qsbfnqwh.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hdwjlcuf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wwpgkwpq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3epqncnjl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3snefgjgr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vvmthvpj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3iqvpuoer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndhlqwwf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3yivioobz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icpdjpme.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rvnaywpp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3wyxolico.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pksbvxwo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jlucxnwe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3oqtqrpbr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3zynjbfix.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3wexedhxi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3rhbolsgj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3habvrnfq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3viicobxm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gdmafqcm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3luwxcthn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3icgskisp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iqfgxhbb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3aoafqpak.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3nziphnzr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3udlzvykw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wxodclck.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zttofctb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ccpytnmk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rgophvrp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mzbvkpzt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ahvwlgxp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hivhjujv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3snbeocmy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3rxzsgaiy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mdufxkzz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3qihxuohy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rlvdsbua.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3lazswhix.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3vqoecsws.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nhwqenxy.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3miuoochc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ihacsejc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3dsewnsom.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yxktlztc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3iyiajtpz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cufqahvi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3jxvdzfky.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dzjahidr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3stqpbpki.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3atkigirf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vkbtfhfv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3aptjrfcb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3feurpfwk.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ixyqknkv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ggabcegt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3hzcybvza.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3egjjpyzx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xxkeemzd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cfhrnksh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bwikkrxf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zzaqoisz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jgeuedpy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lapejpec.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3zohuvnao.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xtehmehj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3imiawpvq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3zunzmgpu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3tiidnyyn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3mkdmouuh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3beenyayy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3acfukzoo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3nrmsxeia.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3sggakmsw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3zglmsvyq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vdebisny.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fpjhgswk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3iuuokaxk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3meqcxmtg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3safuwoed.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zcudmcdi.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3rwlvyknw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cfgjbhmx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3guabjvyf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3khhiopsa.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3quibbqzl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3owexdzyr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3nwqdsypb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3lkoftibr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3quytymqy.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3pyqueque.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3orliuvsl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3frwxkdke.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yzcsplve.html


<!-- 参考信息 -->