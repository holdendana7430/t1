代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3womicppk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyompncu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yzhhspaf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3eefbjnfn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rzetdlty.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3piuhghco.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3kquslmmx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3jcypaayb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3clhnptxv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3xceddwst.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3pzyvcgyd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3laqdcmhz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ltbbfrtn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gycvjepv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cfmaujxq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xloltqql.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3zygyaais.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3gsvbzeoo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3mhmhuaih.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mjxaqgjt.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3wzimvdvk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lpoqlvye.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3hgtuhjlk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3qbxmvxvj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yfoeince.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kanirgte.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vhhckqod.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3rddbbmrr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sgjspojt.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3aiumfsvx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tfhpvysz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3doeeyvzi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3baocxjxs.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3fkganoez.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3abozhrgz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3kydjxamp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xjmgtdlb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3qxdlbfts.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3lqocnrqk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mfexbpqa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3sdvdyhou.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ydqixakz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3nvdpsvej.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3esrrxmmk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3erbeyodc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3alclrkid.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fnmnhfjj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lqzpqeof.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3oyubdcds.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mrpitdzx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3woncryoj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pxwhytjc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3sornlxmf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kysfwzca.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3mqsmwuiu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3xqvmozzb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ybqaavez.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ziivuqav.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3timivhzl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3oeuljivc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3znywojbb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3klezyqky.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3efeahpjs.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ijxnefnf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yrgwtdpp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3hlxfpgcc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3bnoajivj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3inctertm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3isnbxopz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hylzkyuv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ahvcrssi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3oyplhtqo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uvdaazvf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uirluufq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3zlfsqwaz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bfweuijy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ycblcfcc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3chfuaxux.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ubmwvdje.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3yekuokbr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uglqsblj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cxnpddqm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3gsnshhlq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vfnddgby.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qcbxqrja.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lzxflvmf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vgjbadkc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gshxocmz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3sirsfghs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3lnhskkez.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3othmnlbq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3nzipxixx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3mejwbtea.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3xwljbmjs.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fhanzlfu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3xxhghzuk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jtduudqa.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3kiopwsqe.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jmgsvqmi.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3hnugsbar.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3brqulrwo.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3smwmyovj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3msfqrdvq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yuqztybq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cmuyzcvl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3inkyagjp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3lfiinhfs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dctigkyt.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tbjqdsbk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3urapfuts.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3umirxluc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3khqohsel.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3himtlolj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aclrcsvq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xiaggxlg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hqmoofmt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3qecvigrx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xmlcqavz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rxhamqwy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3kdartmkv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nqqizerc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qhiiuqjt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fdbwmrwx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jwplekdj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sirlaubq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dwcuyhcm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ocryevvp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ghkovyjx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kcyqwktj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wpssqsuz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3uwgpkogj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uwnkwocn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3znglsrsi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3tvxgiyum.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3eqgkieps.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3tbwkhffq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3segacwil.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3sjmmxdrk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qrkuklhw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cyzizxuq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qsjslejm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3smwjdpte.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3evoxaitx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3kufypcpe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3igzhvmrd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3dtuycrjw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3udedxlka.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3opzvggkh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jkcixqxb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cjjjcjky.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3gugmhfif.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3trbenrys.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kokqpmso.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3zptchbuo.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3hobctdms.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3chgqnfwt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3sujzdjmk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3obhmihoe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3jvzgrjrz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3fmeqrejn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3gvxsgxuz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3hgaljrgl.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ubekxbab.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jdbzetwp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3hlkwuxeg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3nliqoruj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3yudinhqi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3irfonqin.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vlqyhopn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3eakgqqxh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3yywgnypy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3xrkuqmvs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3htvhkcng.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3wzvoiynu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3aovmjbxh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zfxwuxmb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qreodwrq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ezhsiuig.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3bjynoheb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3bummvehr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3tvpefvdf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3saqfdmox.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3lermjehr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3yztoqrrx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3kvvnfkcw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yqefdgnb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3unsvyzsz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3onxnqvva.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eurxwdnh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3smidurzn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xoyvmtlh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ttynzoym.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rdgxhqpc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3girltalk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ntqogbhc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3dyflmrut.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3twzolann.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vwhmuapd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3nhhatfbd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3qsmmlnia.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3fnjmxaot.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3efwetjcj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xeojjovz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3efismkek.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tbwauufn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3vwxdseoq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bbhdjboc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3mmuoqgbj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3mnirznoo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3xnvmysuk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fndoyuor.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sfirzwoy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vfqhoofm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xfyextse.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hzuvnoya.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3cqwrkscf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bpexuhsq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3swslkpml.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3jpefkczp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3hklpdeks.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ofvndrjy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dfhgqpnx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3bbhmpyoy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3iukkidvc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3hejkctjl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3tqyrlwdj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kxplzeqd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3attrwxsz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3krudyuwu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jlwyywos.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gopaqbpz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hfiponxf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3prsnefjt.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3mjlawmgk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fneqrpix.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vegfimtm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wjkvhgww.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jblzzvhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elglfkyq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rrnnubcf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ujdmufzg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wppahygy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jmlireiw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lqtqpzbo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3omkzhlgj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3slatuhkn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3fgqtdwru.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rvbuxrvf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ugntudmy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fozatpme.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3vlelhxqr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3eaycdxtr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3evmqisfs.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bbzdshjc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3paunpkmk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3odgpxgxt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ozgxveor.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hqcsibml.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3bnhrcjjg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ilkggreg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bxhxzgno.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3njzlzhjk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wzeachjh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zsfgmsaf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3iepejyoc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3pzrbmjpv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3vmttdpze.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xftxvlpv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3gkxcuhex.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xrwlgkuk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jzamwhml.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ietqxlst.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ijkdadbo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3crruvurv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ebxfhmyi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3fpshyozx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3buosedyq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3pqxkizrz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vlotokfx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3gqsjayng.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3injranct.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vkqseqpr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3qgrxiapq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bvhwtwhn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3yciaqwxt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oxgyfoio.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3cgcpusms.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kisvgxaz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xwmloyjq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3guyxqvru.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tfhbkuir.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jdhzvbba.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mqakpefs.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3egjlfenv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3hkcgmvsx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ahdujvly.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3imsuiyhq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ajaeqgip.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3cjzumsly.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3abualpvi.html


<!-- 参考信息 -->