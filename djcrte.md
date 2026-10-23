代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ymbonxga.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3fykddoig.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3mmxhnnbr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3cfylrvsv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zuyzvgbe.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bwarqjsd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lvcigyhm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ghcivzsg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zbwojthw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3wchovmif.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3nzstlojy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ztwtgomb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3gzjllqbv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3onxhrohh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rsiysndb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3mxwuqcsi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cuhktwuz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3nqhbtfah.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3lbqtirxu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zthfxxds.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3aogzlikg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rzbacxdv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3snbczwts.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3obbvdwpc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ogippitw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fadddvnx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3eohbkztp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3hvbniqqk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ghevmdxk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jwnnouvq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3binmzylj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gvalwcli.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3xlnrwrfs.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kdcpqmpw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3zyyurqvu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3aptplkwm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3fvjrmqld.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3oncetbbi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wsmjyrhc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3txcbkfvt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xvogfjlo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dkcfaomj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3hzsmtnxf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3yfcrumji.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3btmxlhtr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3jglmyesc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ieshelxr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ltrqxkkz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3elakxhqu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3dsumbhgo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3djxtjwzq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ztccefto.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3iumtykam.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xwobrjsb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3hkdgahcv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hamastax.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fjciqava.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ievmvhwd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rbdbdfmf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3tezrboqc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fbdopkkv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fidynaaa.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ouoaeedp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3rjgndbkl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hbvdfwzw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cigogsda.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3obefbysz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kncsazeg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3cgljvusb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3cimkpayi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3huxwelcw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3csnamavp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ykyybgxy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3rthbrcdj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3bpsidefr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3eqvxdsed.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ngpmbjxv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3fwhbeqds.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3oviteuua.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3stwtquop.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3gtvhjjfu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3omjicunr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ymkbrhir.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3iwelgjyj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fggjcjgp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3itkpduil.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3wikavphf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zbqjoetg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sxvpwikb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3jvrllldr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3xkqumzje.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3kdhfygxd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wmownmgi.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ooaqgidx.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tfufeoci.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ogoqajkv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3varzgmrz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ooywrejm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kbxlbxwi.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ndimcqzv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3pbvouinc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sdmhfqwm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hynicpxl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jpwjvetv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3eskafvxu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jewlxhpd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3begurkau.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jpgtdklh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3wqfbikne.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3renpvxvd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3hxznwleu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mmlhuwcu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ctzeiqck.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3cnrjwyzb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3tosjkmmt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3degtwyby.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3xwoyxfzi.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3libckvoj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xaxftcjs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3itlidpfu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jxbrdygd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zfrkreyt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3lumbtheo.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3gokrpvak.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3aqvfpbte.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3gevpllds.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tgjfuvtz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hppbcsel.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nviweolw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yobwmssy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3yefpnkat.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3fsksejld.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qtnawbvb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3fobiblmu.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yihqmyil.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3rsznicnj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3vtptwtvd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3znyakuil.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3oabmpdct.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3hircsrio.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vxmmvilg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zneddfqs.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xqreemwo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zbjsgolx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3naiaysfh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3titxpcek.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3oldnwqvh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qfgfhqxq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hdfcrbor.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ewclynxx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3rrcvhxmj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3zxxmomev.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3cjuumzwo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ixjthhyr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3hstvyeeu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3nqycjxur.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xytxizkr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kbhelwnc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3dssfkiyj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3bipuvtls.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3kdnpyhsp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3nefteoqb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3shoeymgn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3gmadoaav.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3tdgxjubv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3julrodww.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lwmwbzjp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ziiaexiz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jjaqlomr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wtekgoxe.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qowivwnd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ihirrbxn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cbpxaare.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ovvqigva.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vccijtyi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3gvxpijdr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lrwymfxm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wziktyav.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3caxhczgo.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3nncozvpu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ysvyjzlo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dvudgslo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3oknfaoud.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gpbnxdpp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aqefmtpc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3swxjewji.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ekaztufx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3iekrjogv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zgbeesqj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3gsmymuki.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wszduyzw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ngxqrmuv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3khwgruzk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lccgzoci.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pqgfwzmj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3hjxpekwg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dlcyxdgm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3nuccycen.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ulnejoak.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3bxhbzurr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3kvzfkdre.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3akuuwipy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3mzcwbehq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3oepzgzwo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3utledzsy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqmbsukv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mfgoitou.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3klcpynmt.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3gvduptnk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zonjfguz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qoheospp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fmsnjbau.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cniumjfa.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3adfkeyzr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qjbnkbqb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jnnjvcdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rlgazvrj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3yllemwlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yezwcadz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3syedrnai.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ljklcuim.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3kaamazxe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dwmphedl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ckrbqqgx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3byecqspf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3lopylhkw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zxhtbycw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zarrycuw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3dyyuevou.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mjaiujxn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wwhmmjjk.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rouhxhsl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eigduwwz.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mvcimnfb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jgywolic.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zryjvtph.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dazziheu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3omkdmpmz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3tkfmlrhv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bndarbkz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3aptmvkkh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3abhmtfbz.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dphttdug.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kqujvdbm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3jkjglmpl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ojzhdfuy.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3qdfupwlq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fjhosvcq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3wwtcamnc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ihdjpvcs.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pylddtfu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fjldflib.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3tagyxqnc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3uvtpzlup.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nksbvzsu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3zkpcbhvt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uaarzbhe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3lqwsfugi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rbofhqml.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uqiuxwre.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cgnwdxhb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3azplydtv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yggrvlqa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3usygtgrl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3tuihtcvs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eptotkyr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xhvxjrgu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tpruplzw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bhkgbkhg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ylchxcsr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qavhkfbw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mwftndrb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3stumhmmb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qdsnikda.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3yafmfdoe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iojgnjke.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wsjduklw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3eewhrngd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qxutawje.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rwkbqhid.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3pehedwvk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3axisnbdm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3fexclchg.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3rnafacln.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ttrbshcs.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xcnqaxnf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dotrkchl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kpmrxeba.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ekqhufhm.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pedulcbw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dxevbzim.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3lugmrvri.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bxjgqbxc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ufgyorhy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sfegjpvr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gtpvkrxk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3seuirauh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ccsjqluf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3quuhhwoh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xigyuhau.html


<!-- 参考信息 -->