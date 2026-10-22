代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wwumvdqk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2wcknnzwa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ajngxjxf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2szspjelj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2gvlinphf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2cezjiose.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2omfkldgz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2caolxnqb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gltoplrg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qsvsdxsu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2lcnvevwk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rslkxbdi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pjicehdb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2eykztinb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2rwkxfjrb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2bfopgahn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ikkojkmd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jkhdhich.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2khetsbez.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2grhdbqbv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rzzxpuzd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ujbivnca.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fdxahsvp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vwprstca.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2emnnbles.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dhpkotog.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ljpzuusu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ajtvacbm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2cglxqofv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2vpezazvv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cdqjwuxr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2szckqnbv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dktqqmkc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fwlupmja.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2vohnhiur.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2jrveejwj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ryfmwlab.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ebejozfp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2iohtdbqc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2pqrbmqab.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2vsyffdfw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ulmmdscm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2blabfvlg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2jpaktkyx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kgaqszwp.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2viprdacl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2xbpbcaex.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hvaotyji.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2enazyeca.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2dxzaravy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2faqayimc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2cjwkfeaq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jitmxetz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qatduaqr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2hreailtv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rjnalmos.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tcngucgc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2emtygruj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2brdvpppb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tgbypbnz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2yqmtbgtx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2kctfsmkx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2qcjuiark.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2prrjdlmb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2sruavwdt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2zcqubwkj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2atwphyse.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2mfzndpyi.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2daiozflp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mijiphjx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ogqeumlm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uiznvigx.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2lkzacgjp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2uzoxvdbo.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rgcmpprm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2izamdphj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qxbuafjt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2skqkzvkv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2sfclzwnw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pswbusfl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2sogijosj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2wduyrnxs.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2umagzqfh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dqtxelsc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kgpnindf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ictaorom.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jnksvotq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qazwgidf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2exwzhywn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ouqboqcx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pidkerrx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2qlskgkmv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2guepoiea.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pewklffi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uzxficlt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2msfdisrn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zfkpdhka.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lkzqydqo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2svfwvsjt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xwtitkfa.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2mzqyayfc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2bvdfnjie.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2zjsadnva.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2cvjzbywa.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kakuager.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fccincap.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2rfugaptl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2dfnogtok.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2szwfvvmt.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2awaoslcm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2byvebevu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2harhrsyr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jjledlco.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mjnzjqnq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2uegqpbem.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2wryfgyop.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2vgrinedh.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2rrzhsvfm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cfcikixx.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tanmvjkt.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2grokuoke.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ialsfyty.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2frqpnkvi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2fcleywvi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2henaxicw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2hcxbgwap.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2kosjrwrs.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2unnfrppg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vqplumtw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ziqthfqw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2vexxbvsx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2mzvguiee.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hlnfierw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2bctdlzsq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2xdagxcse.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gaufhthc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2gftdwslx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2whvipgiu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2etjkrhjv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2bwcracuq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wvhvzfyn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ggjdtgsd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2wosyhzaw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2kmcpxbkg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2beihskgf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2bgrzxlev.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2yzbeibgj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2xuyfrbae.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2cbiaijry.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pieyvwlr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2wbfxgujx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2bvzdjgrl.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ahcsqleh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2mafctako.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2mqkcdfmu.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bmovygrw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2dtuyakth.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tadftlra.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dtveeamp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tjkwviqf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mcroihxk.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qatwhwgt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dfgxgedr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2gmmpkyeg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ojbtzrhs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2frilszcd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fwbulibd.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2myrarrhh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qhpyjiwf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lqiixcbm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2defqwrfr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mqzhabjc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2odjphmvc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cjabvdzl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2axnljfhx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hmafcnnj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uuqrddmh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vrgewegc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hwrsssre.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2fqbvbhjw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2fzonkxoo.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2jxyaelbc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2yfjxziqi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sikqdjtc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ikavtthx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ctvjbawv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2suswdwnr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2vhovjzyc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hvoubfks.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2soddvvue.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2xlbxnhjv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2yiemtuof.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2lchbrpwu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mwhyyptf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2sduaqfyn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2sxzwptvs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2uthmrivk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2jbjywxzm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eondxikd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kxubnhpx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2estjwdhq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wkvahvfs.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ionzmztj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qrhlwlzw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rkscurkw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2uizscqng.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2owjywydn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wplfwkfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hilrizgz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2vvgqvzkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2taoruepx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qbikiogz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2yggskxli.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ztxtinbp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2noulvdsx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2itfcfads.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2qflfvvpi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2zmfgvbbg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2pjcbttav.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hqxfkbwv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pysjcxjo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vnyfjtjm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ssfqtvce.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nhsswbbi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pctxodcq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zmtjdnve.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pcrmblex.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2pkebcmdo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rsubrotk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ndlpmzuq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2nufvrtgp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2umknewvv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2udmtikex.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qcilmdny.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vbcctwst.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rxestwwc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2jnmsjmal.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cxjxrkxb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2wsfkoaet.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pyhjccoo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2xkubbxqy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2prntoffe.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ehatwyeq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ymljwxse.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2qlpbqlfv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2shcrlrdx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dnntjtjo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2yesglajw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2unfgcxth.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2wgwulihe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2apjcyabb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2erdipqll.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tljgqimc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2rrrsewau.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ffbbqzwq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2edjuzpju.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2tbhxxtzu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vkktwafz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ugdjplkr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xmazcmhb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uzilgrim.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2svmtxwqb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qiggsfts.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2erljpchj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cxxyfwdj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2zzfkylrx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2voreqqrc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jepvzmji.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2vifhlwzj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2zmzggonl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2schfqtqf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2onkqtgei.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2xadsjjny.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2zgmfqgiz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2mlhjwnyj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2qdwcqrdv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ifehqrrs.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2avuivlvd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fdjqdsrp.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mtbppsdz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2jfqgrqfe.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ithdqesr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pxhitozg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2jbbtobyx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2jhubkitx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yukdbnrx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2atagcfex.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dcffszlm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xrapoiwa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2yevigtzn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gxgiighh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gvblefya.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2whbkikif.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2haqjvpps.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2xwmuqtuw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ndtikuqj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nvobpypg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2epnjelcd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2uloottfq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2iboxndvh.html


<!-- 参考信息 -->