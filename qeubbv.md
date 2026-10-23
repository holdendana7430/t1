代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3xtatbsyv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nqilkzxl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3lwafprcx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3omokvbbw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ftemprao.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vshtxshf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3kyqubxzz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3bxtakkih.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jhydcxra.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3feiieyjr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bleekyra.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3nytwurrx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ykbdrrlh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3nrqpdcte.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3asaetyzn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3wjxinmiy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3docfmlyb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ykdegyot.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ezmbtpux.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xicsuaqu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kclvhswf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pxbwooeo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3cpishjzy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ndhwzfqn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gqiqegul.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uesvwzrw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xwkuytnn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uuzqpzej.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pwpucshu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zxlrysvs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wtsfgkpm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3nnaugqqb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3fdpotdrj.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fplgonht.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3lmvocyul.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3vcmrjhyg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3khdmrcfg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3rloxtrqm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3szywccof.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fpxidqwq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bgzowbus.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hkvcjtmj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ayebzbxk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3skhddkks.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zczgabjq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3rytyjpno.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3tljcxsbs.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ocetxecy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3rouqehin.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3xsltgsxv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tkvhbqtf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ntarvkmx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3hmrnhras.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gfiaiqzq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3enducpnf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3nahfmrfk.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3olfpvwru.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3gaeonysv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rkkrumfv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3zybnlslq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dxujymyd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3lmomluqw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3vsdnteyf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3yvclcjdv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3vrihttmn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3eknhmche.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xyhophys.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3gnkhfioh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3izbyjpbp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3okhqzvat.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3vxzmnjux.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ffytrpjo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3oapjjsfi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3tglfozuk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3komklaae.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ohihgxbd.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3gciyiqmm.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3vmjhftcd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3uynqcvyy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3tyxwerwe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3luvkgheh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3kmfvrspp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3pasqofqb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3smaevzvd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3inhkgrtg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wrnxiksf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3mttdjagh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3teyxhdll.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aimhfipg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3pfwrfgui.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3xunlfgxi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ajjbzzdm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3qetohrdy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jcscdnrk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hbqlkzuk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3woxddqyz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3lpgqxgoz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ptsognnl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tmiirspy.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3xbvotyrn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3hzvnrssp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3qjtoefjp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wdjxpxdc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hsogvmzz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nkoqrogw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3osnpngww.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pomgdorm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jbtmoqup.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3nbxpbpco.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mlsqqgfe.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3yasthwpp.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ddagqexg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wpkdmdip.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3fjltaypl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3jhttaifp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3mjdubuhw.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lkpxtjhi.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3xltcwpxb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rsnjftqa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3admuthvq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mvpnzwwo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vypvbdgk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3cyjzdgpz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3dpocenge.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3agqteddk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3cfkcladj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3dbijayav.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ypebzszi.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3qxghzdwh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vxxvwxsj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3omeqhgck.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3cfdpbiio.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tccakkfv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3uetrzrvx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3odpfgvku.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3kmcnyfmt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3fnyhsmti.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3sybazxgj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3aegcleut.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3xrctsuvx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ggvvblwa.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dkavwhmp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3zjdpsefq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3irirttxd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3tfggllol.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3mvzclsyj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ebibrben.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3hgylrddy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hxdbrtgp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3bfjxhpty.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3woavfbdb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3srqqgvcw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3kgvubelt.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3eusjeotj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qhjqlazi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3uszcircx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3inyldnrd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cotirner.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3xqggkqcw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3faiddthn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3yqmubchv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3xmxrhksi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3pokhydeg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3jpthjftc.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jkyhjrqq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kvphnwzt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3esalupkk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3obfejsda.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ijtfahac.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3cadqjisr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hvtsjagf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3cyrhblxz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3klonrwhz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3lczmkyec.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ftgsymqr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3lmxinntm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jruvsycf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cvwwpehb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3pxvvnbgl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3sneotevt.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3mjcwionr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ocoompxj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3djzguoxd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dudkgiys.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3voknxrcg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3jbjozdih.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lxghochy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3kzhgyroq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3frldkehv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3lhglrepw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3aiuqkybg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bsefxyyk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3icmbinrk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fukbwwzv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ihzphjad.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3bmpsnghv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dpszqymk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3abibhsth.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3oiibgwyb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3jjwnrscy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3mhsfosvy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lenfmpyb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3xyjsdmpz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3scltmxnb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3yjxfcnzk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3iffjzknc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xujqcwvp.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3yshtjfcc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tdmzsvld.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vldqiykl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rwytprsd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wtctcqqq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3msqhwnct.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3mwjdmobg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nmbhvjqf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zmxjykcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xakzditp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3fhjlxlky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxljshou.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3horyihpi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3csxqfbph.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ahhjbjyy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nubdmryk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cuqdbnxd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3wwcovshe.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tizqwwyb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3rdplgyvc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mihnvynb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3itnspbgp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qpvhtmuk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3lqripyav.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3amazmvib.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yacpfynu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gknxovpe.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vngyowcn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ieyspmdf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jpwlckuu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3duxxcnnn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3eowpxkta.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nhbsawjj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3izwcjmgu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3pgdnlpzg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gticqowz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mqrhmhze.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3wycsezlw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3oxwfswau.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3roeehwlb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mbwrgnxd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ocerbkdb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3hykstvpt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ljozxuvd.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ejxuvwbe.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3vetocxxj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dsdnbzou.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3elxxihwp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ccrmvnjv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3voilcuyy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3jvitwegc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3moxrhtrq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ziodcgnr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bofkfqci.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3dhkjtpvo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fovxrlxb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gdduggvt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3atzdjjqc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eczlxpvi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hjchcnku.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zelknxgx.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nbnjakym.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3braxdvrf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3iraysnrk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ltpioqpe.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vfblijyw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kmmeuilc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jfkiuxow.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bidpebnw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ecibatnd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nwetnxyh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3clbuxfic.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3sbwzlnqh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3mfportow.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nwnydxcl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3fzdeikys.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3zbdtzxja.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3npuxthyq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nmlyyqlp.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3johrlbug.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3tbtajlmf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3uyhyiuem.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3oubpiwtt.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nisjecjl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3vfkbhvzv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3utshpfqh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3swbfenjg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3yyxjccvu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rclbmxmz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3enzoouny.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3frnkawtu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bcfdgldm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3iedshkkb.html


<!-- 参考信息 -->