代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qpihcrzt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gcpqqjzo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3kufsmlax.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3svodxikm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ixlzbgdq.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3eykwucxm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3vbrsocke.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3pdvotrkz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3litxjdnd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ixcuvfii.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3alaalnph.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3eqzrmoye.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jardyghm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qvxzwupw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3sechtych.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vhvchbaa.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ecbgoacd.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3oevomzvw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ntaazgcm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3uwmswnnx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3anpgafzl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tmghglra.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ojgfwizs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jrbddegk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ooqmiaep.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3jinxfxwg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3tdeacbqk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3pejgllzw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3hldkkbdy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3uhmlrykx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xbrrtpru.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3abeoucjl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3uftzuhlx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3featjpmq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3stcclujh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ajevzjsw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zhswcpea.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3waukmsyo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3odixvjkc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3yrxxzsgy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zeowjmsn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dxceyhjw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tfnlkxbm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dckgfmrn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3poxswlnz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3emyjglzb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3reetkazw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dzdfrfor.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3gjbioghg.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yihbarad.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3lxparllx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3tluziwss.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3jrimxnaq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3yszwdjch.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fhvrkxam.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pzkubpnq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uzcchftf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hkvdlkoi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3dofxslkk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3pxldzkxe.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mjapfkut.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ssgxpcxa.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3botdenvs.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3nvoaansx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3hfwdqgxp.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3dtrclovh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3veeywwyi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3fzuchrzc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fhrvjavh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qqobyaux.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3kmlrfrpu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bxmmwxna.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3mzvvnord.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3pwbkwdxd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3baxnkllp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3mgonrijr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hoxiajgl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cqmzlruo.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3uxvmlvdq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3oekdwobu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3avaesekx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iawuafuo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3sawvgdbc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3uozmrdnw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3bruedquh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ytocgxvx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3zjuypndf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3vuefoifg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3lszqpgjl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3puivisys.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3hziybjms.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3zvpxjods.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fpknkqda.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tnjxhzhz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3yppedyen.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fkxfleco.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3nybfzsvo.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3lszxveul.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3xvmpgkda.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eqkmvgut.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3myzuirnm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3tfqbukpk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3qgwpapnn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bmalgqmj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3dzxgwfue.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3uikaislw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3yenbfpeg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3hgzcbdlw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jhtlrdfy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qjqiyrtg.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3cvtxjieb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vmupjtnz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3rmopnjhi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3qghxlzvg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ewjxbqir.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3mpmwcpno.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3lglaliyr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3twaxufyg.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fcmwzkwq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ekoovguj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qlmdduvk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qkyhfogu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jgbyrwyv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hzemfsgd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3zeoplrru.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3enucpxib.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ynjcnehn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3trepbtlm.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wyrqwnsi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3luupiqxp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qozbgerc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3cgkvmrfb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sfjuqwgu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3tusxjugi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3itlyvpis.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rizjhnlx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3skbkewgq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3unbcrefk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3nuzlnbut.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3fhdxtxyq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ndptsjjx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3vmjqajfk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mnlwusth.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lxapagrp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3svlopvqf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3eqbeueeu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3wwpbnxhl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kvweywpt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jwyqiupq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3yrdhusvy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3cocdtcut.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3kublelpv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3psqquvjj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3jphcklsy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3satdhpix.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ulbyufsb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jghkyvpr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3liluxgze.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3doaxucmi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3brcuiflw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3okxuvphz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wfwfpjrl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3vxvbzuvc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3jjxxxkqo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pwotwber.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3jsfvaofy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3wfisftju.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3hpjypngj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3wkictmgp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3wezqsosu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dvtyfokh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3rnhiworo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cvvmuapu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kxxlgfdw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3jtmyhdbr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ofgfekgh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3nzoicnzv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ypzabfwo.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3qiopyxbu.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3aknfzdsk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kahjygeg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ojvqwslt.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zcwnzguj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nxsjkacc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xzlwjuog.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hghiqejo.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jtixruqc.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3qglzagkx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3emttppxp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3qqkpfnde.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3vwbcfptc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3bwetpjls.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3hnwsxukz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gxsusyuq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3hdmykrfv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3adybfqdn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3yicvvpjd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3keheksyw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3oziorqfa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hvixdypo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xrktvbqd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3kojhvesl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3zcfhihyi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3rhiyjssj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3jbloeefe.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3dodjbnlb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3idxiweza.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3dwwipstu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mdklmukc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cxaujdhu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3retxtllt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3nubqrjse.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3pamhzjvg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3merklruy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3giyvzmyf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3wclomhhn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zzxamqwg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3jmkefxwp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3nghsywnm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cxtxvpam.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3iikgrjbj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3csaieqza.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ckkqnkjh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3zkhsaysn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ajvkklbv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jecsnlqz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3itfutmgh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3blkhbzfe.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wufqbwdk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3rfppdwft.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bonefjqm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ggowiquy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usuonncw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3tkrezkfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxyqpqok.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kmklrdjx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3yctiwzxg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3rkzczowk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3djvjefat.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3oisstmqf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3zepamwta.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3uehgxxtr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3xwicbfiw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bcbomgep.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wizojpgl.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3woagpnlb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3smziusyx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yxpuabwu.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tmchqojs.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nzgoezvk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3jqigqteb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mmeipinl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3bbctmhee.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rzeengcn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3tznedgvt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qmixcvtf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jvvzpiyp.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rmkswako.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cftkrawd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3utcrupst.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3jvwjqhyv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3jpzxoszm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3eiqduuxg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vdejfhxk.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3eykeyrgg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xbbychom.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gmyyzoib.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rocgjvbu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3khqelvkg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yxhqdqwq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ccnphhyn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3jidhyesh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rskbxzmo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3yxovjako.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lhovvtny.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3bvooecwa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3aoiroqrg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3whkdudjf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hslhoixp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oljgqmok.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3gyeozqya.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ztttfbzg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3psvsbvza.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3btcyfqvb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gejsdqrs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gdvndosz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3odmujhmm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3taysrdms.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cjnzusxm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3dzohfmsv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3cxzafuaj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bwxyfpvw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ownhgase.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ubvnzeil.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xmwafcny.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nxofvkhs.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3fjecovxf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nsvqsxjl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3shogrnto.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3cxajpzlf.html


<!-- 参考信息 -->