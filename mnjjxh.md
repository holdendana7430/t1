代发 wailian999

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2lqnvssqd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mmfqbccc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2hjtakswa.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2tsxjyuyd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2zmioakzb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rhjhsqwj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2pbqhilde.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2bepgmgqv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gervpvlb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nouafgpw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zkpqdmsx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2kmbpozky.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tjtvmdzf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rnphwluz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2daxtfhdu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2kztbosht.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2bgmcrjaw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wopxsend.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zyczukkb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2rsalwdvh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2umrtlkfj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2toztasie.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wqnbxmeg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bamngctp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mbfprueq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ynapexte.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2avjxlvas.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2inlkbovk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dnxqnfjp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2necpvzut.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2npzwqvpf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qzjfnysw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2emqzkuyo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2inhhcgwx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qkpiqsed.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2fxuxveac.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2mzjgzuum.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xdcntfhx.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mmfzcgps.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2vdnqbsog.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ppdnseax.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xysbcpmr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ewuvfatk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ypoubcmw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2syezvgfw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zsfcqunz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2pwcoxqls.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2kwbfnchw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2bkumdmvi.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2uvctxfjj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dzllaeat.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2nitgrrid.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2qfdqcgkx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2undbpplz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ivprhbzo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2hsgvnqfh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2fmuibsfx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wuwzwvut.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2bwamithq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wmsssuwl.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dbowxevx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2hrpwgdrj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2rgrhcddh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2dutqqbdf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2khfqslup.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zhaqpqsf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ijwhwhox.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qyfxyovq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gxibmdmj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2enftanaj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xpbcehnp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wizkpxza.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2gtqmlxgv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2uwevcllw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ogctgmio.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2bqdnebyp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2wfxubdeh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2lqeebosc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lrwsakur.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2vmhryfgy.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2eanvpkee.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xihpiudl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2wzyqdgbx.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2serpqtav.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2aviqksxv.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2tgymzpkv.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2dxuauxni.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pmjunizj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qgwyuznr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ecbbmuct.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2jzvaaohr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zdjaokfp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2elsigsai.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2mksvskbq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2jaqlfwij.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ifdjrhfm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tkomdjzx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tvoxphdb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xjvvhlmk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2wjfugmli.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2npjdajjv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2dgswfpxu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uyfvgzlk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2rxfvagtc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2poayuqwz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2npwfiygq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2teqdiysf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2slvqfhxx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mrynlroi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ndsfodbj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xbiatcth.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vkmngdfb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nfrhipgy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2emylpvpe.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ifrtidco.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2asgnnlql.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bkpbufvh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ndwqrpps.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2lzxxvakj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2vaoymroc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2gnnvycfh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2zfjseqwx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sfbwbrap.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hgfxovsw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2urqpzpfr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2zeffesva.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2imuorlpr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2admqhuom.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gkmxicil.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2clvglfyr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xrhigpkt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ultenphj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iihffrwh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2rtlwucfz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2aezlrcul.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2rruvgeik.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qeyjxogn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ithcpljt.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2fkreejqe.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2nzowgkfv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2hzgbqfcl.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2dxsenakr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2bkbwpviz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2elvfzukl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2wmdvkeai.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cggejqge.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ciwmksic.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cuyfwbcg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2tachweur.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aegejqam.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2mbnjkawx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2clobckbz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2pewnoaqp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2imiifhhu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2pdwfysml.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2cjjdwxwr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2vnlmwgwk.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hhoyqpxf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2kgubmnnx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2viwzrutv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ccegzltv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2uddzmupi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2lbdhltas.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2wnbkjfyr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2snltmjsh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2rurscney.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2anrhrbid.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jqelvmhb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ltbeegur.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kprhkrum.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2olrnycsn.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tccyoqsh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zgxjwrex.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2uatmjqdg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ziwcddxw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2njmvqjku.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sedduzoi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2xehanmha.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ymqcoyut.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2hgbcxxye.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2boanwubl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hakstrnm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2hbbmufzr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jqqdkpxx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qgsvxmul.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2fhirkkkm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2zuejdooe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hxqcxjyp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2flksitll.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2hnqhvddi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vgdmavpk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wkmkdmoo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2jidqrkly.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2exwznrit.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2rqvugjzr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cgmylvgg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vstyuniv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2myvbkbus.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2odzkyphm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2hdhslqjf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jtqdmdqh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2tndkaylo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2fpchbnmo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2tawlmymk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ffuzpejy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dscjsmcd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ppxduzhe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zbkjvnhb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ntfwlswf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2mrvodrer.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lijpezif.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aammfdzx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qxmisbpu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2uzlqufvn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uyalvrcz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vjwapbqz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qbjzwmnu.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rypgsznj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ciatgkll.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2yoodpxuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgczbzsw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2zwcjajrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvtmohfg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hprvfeca.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2zzlngnpk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2cfagpfhv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pftdvirb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2erjlxvhk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2cqopfyqy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dlhvbwsh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2oqyqdwsm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ulkuyvxc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rugyjkbj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ixaddgdt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2yqobjmig.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kikrtkaj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dbbivqwk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bcrqccgy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2exywbkkn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bhcibqik.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jipdkimn.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fpbamydx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2zrsgrsek.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bdcgysng.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vpvklgje.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hztxffjm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aiheneaa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hafznlpx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2vtimwhuf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ulxdehhb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2urwwisvh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tbnwfvwy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2akbsbvzd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2mtpnkkns.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pjbljkxl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iubpgjbz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2obkywnnc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gvepvcam.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jwsysgck.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2mexusrnv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2zvjpbilm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ztkicivi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vjaavsaj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ltuqlqvk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mdunrweo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2vxjihgds.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jnewlizr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ukifpcrz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2tmgdkpbs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wpdfvesm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rpfnuvyv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dkebutqg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nkjquzgf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mncymufc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uasjaqdj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2udpokrue.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aqgubqjm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2abmemahe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2qcaeqxyj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rdnzeptm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ypcbcemh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jlqjiayd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2sjebsims.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2phuabcoa.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2sxekszhg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2tdocsjux.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2lybaapmf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2tkpwmfvt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2mkuulmjl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gndcxkuz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wkgzruqx.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bbgjugwl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2wagwmvhz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2woyxnjan.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vyljlpae.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2cmozwtsa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2olutxieq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2nouebhkw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2tyxsbufx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kadkkwww.html


<!-- 参考信息 -->