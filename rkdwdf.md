代发 wailian999

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3slxqbvtx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pkjihyva.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3vrfyzaxd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3srzclvdz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3nbbkrkob.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3lugerluj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3mlsfbnqp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3eyvtbixc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nfletodd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sltiothp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3kedtxsog.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3utqnxycl.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sxalyarx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tomztjzm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ageayaal.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3nhxwdivz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3hkiuhxop.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3kyvmuqjc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3gexrzwco.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3bnjyloic.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ecxcnmpp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3jvnuwyhc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3cowajall.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vrfwjnog.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zdqkpkpi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cpjhgchn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3tfvimaqy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3vyiotdha.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tqxjngvj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3miomaulu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fndcqszd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mbyjmlsu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mwawllzv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3fiyxzneg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pminabhq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qnaizrlr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ycjbjtih.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3srlbtrnz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3yqkvjonf.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3abewfxet.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ypsulebx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3bzhymwpp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qrfifkvi.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3iexfdsvx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cgyhmflj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ehyodmfh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ldxpiuvo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3eduxwvtm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dfylsrye.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3evxrtjnd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3rrhhieuk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3zwtsrjor.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3cjqlkpfd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3vazcrgzu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3gzhfisll.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3nizcpqvn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3dxagednv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3onqicczv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3cdrqvzqj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3oraymhnv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ezchssaw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ligjfpbc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3grgstjhz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3cydgizge.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wgxyocpy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3lrfgmyvm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ledwbwrp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jyncmafu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xfhjbxqz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wqdhlptt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lhoewalh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hekwkdvq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ewwqcrsb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3vmtojoul.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3mmaognke.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3loblrxom.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ukgqcder.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3svgpjqey.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rigslbgg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3uvcyujcl.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3vgudlimk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3anmlzolm.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ocqstykl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3okjleghe.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3zyxvipmh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3qjqyktzh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3uiaixqxi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ygzgepvk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mdbgsvfg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jdvumdms.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3cdbramsq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rselujpk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rjafnlct.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3lwholwrm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3lmqmpums.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vkuesbgm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3xdohumqb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cfswioha.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3leantiuf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ppkryvtk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3bkeubrar.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3uadvlytr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yrgqxojy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ylozjqti.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uaarmtch.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jvdgrwup.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vtnszonu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3keisnssy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3pauujzak.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jttirsby.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hpdluhiu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jfzmbxag.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qbeujkpo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eurntnlj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3tmlpsamm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3awxbwtbv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gxrhohwz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ygvfvsqn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3lpvfohxf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3juebprgc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sftpettm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3pwxgllso.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ghjxtjtw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rvefwmzg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uuhvayha.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nxdufdsb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3tsdxtejf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3zekqdrop.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3akvukfjz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3irdgyyvo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3jqldhljw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3disoauwl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3clhqlklq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3wvunvfpu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3rpjexlra.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kxstikox.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dtpkwqup.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3csgrcdzt.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3hzodslbz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3kmsxflvw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3zpwxscwv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3lifevgxl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3lmdyifrg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3kdlitkiw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3aagegpuv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3bbdfcnym.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3scebpkya.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xfmjofny.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3huztxwxl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3canvtiav.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3bezseukx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3hvdphikq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3sqkawqoj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3xfqezxaw.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3zqljgqrh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3dqlrtvmq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3zhcerljj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3flniwhva.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3frcutygp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ocxvbrzc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3pcnrrrny.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3owtcbdpw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3tsgqwyxw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3jfcumkar.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ocjfdyyv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3zddhdtvw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3rpgmyoya.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3yzkxhmxu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jkaqqhuo.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wrvvdpqz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cgacrrll.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lqtvskvj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3conromec.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cwpyusgc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fnndqmfy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3piadyhsa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pjtkplrr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3dirxupff.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3zkmhzspu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3azzwagve.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3abkguvoe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3uyafxjzp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xxroqycn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3vdfrfesh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3tsokergu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pgfludku.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ptiowkwa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rrseagrn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oidcvvde.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3nfejvkox.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lfkblzgh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3rrlgjipx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3uextsgsq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3omdjrnse.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ihduktpa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3jxiaovzv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3inntcbme.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tgsmzlyx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lourasgw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3raiwoydg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3hfsbddgx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3apnepmyn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ktnettig.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ptxxrecn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3jcftfonj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zhurmvrk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3puxjttvk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfrsuyrf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3qqedqrbb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3pbzxasgt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3csxmisit.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ukakwwrj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3umtgfuyd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pdiiufee.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tefzqxgl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rblatrpj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3aeoskeeb.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3utbxkcxx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vfxulmkz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jinnmkig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdeowmpc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3eyyfoxcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvfshzbg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3djrenlyh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3fdcaqfcm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vzvnmnwr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ixdplqdd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3byawdyeq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ydudeeoz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3jewtknby.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3flmyicja.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xfdfkhln.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3okxhldeh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3frrcibtv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3pndlwhfo.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qkmlpclt.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3msaccocg.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dgpkxlnw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3wqmejhmr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kzaywyxv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3odilrwkc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dkpklvou.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3vzjrozfx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lfgyegum.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gahzmbrs.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tfaduman.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ycjtvkvf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3apomqakb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3drlnfnkd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3swskerkt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3mwqduiqs.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kwebudde.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ucmivmvp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3skgufzdj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3iotiwczo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kfigoptj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3xffvhidl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zmhmixsy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wjyucvsc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3dpzyzccb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nolnvgmu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3utczpqye.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ntxewalf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rgxqrxum.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qvhcmumd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3kmlifxmf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3okwxdtzb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nvhwqvkx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3oxctmpnr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xijgznrc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3pypbdujt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uhwfshqa.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xwruvdmt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3envttouu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhbkdwjy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gihwsicw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nhosieum.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3swpjemxy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3nzfeuizs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yazypuns.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vsxwvdji.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ynujxumk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3yumnmjij.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hehqikeq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3cgwwbbgs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3qwrlkzpk.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3vkrsbthc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3uhvvpybt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3xuykdrqf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wmzyqrzm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gndbfxth.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3cpsonqbl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3lubkuypg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vgaccmmf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3bnintlur.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3nrbkhtge.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3yizruhei.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vadrwjyn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zbybmujg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ndpizmwx.html


<!-- 参考信息 -->