代发 wailian999

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nclfzapm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ltloqlog.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qynsmxjb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3kljibunf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3qgwjvfdn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3acgwwaie.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3itjjsxfs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3cvwwsqmu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sampgbqv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zicmputa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3eegzonia.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3nbgarosn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mqfmttrm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vjeactub.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xhmnhmma.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3obxknzvw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3hhgtgcxz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lowctyeq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hwmndcnv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3oywgcxyk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3kxhjfqwm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3vdxwmbuq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3xzaweyex.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3upwibmol.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rqtqejkt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dojymyfd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3dnbfjkrd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3jpuzekxh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3alusvicy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hvhuoegh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ouytvdho.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qqgizkmd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lrigtuls.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cnufgrul.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tylbxhdy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3edswpahs.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ptihcqxa.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kfphyvzl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3tddjlars.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3uqiwssdk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3cpbblrhy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ruubrcny.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tqkjoxly.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mzcduwte.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gasfoqdi.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zaoivwvv.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3iyygnjdb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3bvgjfmwc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3axlkozcg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ycotzole.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3pidwxbpc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3kedxkids.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3dnydhnbp.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3vxahnheb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3giqspakm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3qsqqswua.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3czsrqfva.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3owwyedrp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ackypclc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3welnztxk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3wqfpiujf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3awycagur.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3qnbolnwb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3xjgopfzw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gxdidhxy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bysbqozr.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3bbyhmihu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3fpbnwltu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3klckalms.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3geopobkz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3aallmciy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mgomwpyx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3jdmifctg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3axhyvhij.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3vdgvcarr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fcpjfbev.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ivjuruwv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ntqjrcmm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tuefvyrc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3lstzuhod.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yceuhhct.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3bayqlnxz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3yxouxedb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3qvyvagtm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3lknlntrm.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3mnzzuuyv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lbgensnd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xgobrufx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3phkqsphy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wwscgwij.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3othomwep.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3stqndddp.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rncpbkds.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3iibphaza.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3rhxdgcdf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cswyfiqi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3qlejieph.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jfzieqvc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bshjegyb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rutdxrmq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3lbzfdmng.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ykdgvguy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zzxqveur.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3frcqrdjo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3fstnazbe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3uddrwaof.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3riqvuxre.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ujoivumt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fxuwwvmn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3iwksszat.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3glcxyade.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xlqmycog.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3kfimmabd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vfkkmays.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3knfmyiem.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hsfcneum.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bmejrbsw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3qurxjyio.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3jtkkucuw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3blfyjyaw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3sqhwkcvr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ouklxibz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aiqxkixg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dfdqdhgi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pllygaeq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3miveneyk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3jwapppdw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3kmzqxehf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bbndodep.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3rcubpjpp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3xrzkupyq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rehsdjfp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kdiyelps.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3jghenrpv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3knumcoza.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rdvslcdv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zzuiozcd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kycopvuk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ialwzitc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3fonrneaw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3vfsojjay.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3phjlsutt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ftshxexf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3opfyxhrb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ifuzhkos.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3pjfvmkan.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ouvomafv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wswlffdr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3neljbqnb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xaakqqqk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3gqbibnil.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3btejqhhj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3eaksdpon.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3zcbdbfzh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3zxkzewfm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3zqulmbjv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3egnkszfs.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3kaghbcvt.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wrikvffv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xcapdrsm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3sliblncb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3imngjimt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3yjwijnfh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3awoznthr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ejjwkidj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3sakusake.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3alibjqms.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3yzlgpmfl.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jwrovwwz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zgqxbwon.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lpmwipgx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lfoyqkfy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jshaejsp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fpknvlls.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cburudbs.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3jprrtzjg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fmxhcopp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3nsholotz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3vgrzvvke.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3hkbhrrkr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3etaeukxl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ajcsltno.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3pxntrygy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3prjhvlmo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3oyhgycwr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ghxusyqu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3glttfbdf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xfbsqamy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kkftzvwg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hvietkxj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3yypwbdnq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3axfvgctx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zaymfqdx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3nvyulzga.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3bovyxjny.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3chfiblpn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ghcisnfq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pyupqxkq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3mofhixve.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3jnnzkirm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ipwpdwoq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3qvimyrnh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3lyurgjox.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3abxsryso.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3qgromccr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3blrdqanp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3cvfxcnfe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ksqyypdp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3uwmaxlnj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kxmcwvof.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xcchqvxc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3xsbdpszd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3huyfwzjn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hlxupwhq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mcpajdlo.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sweuopin.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yuzlinuz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3nqexhgma.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wrdiszwm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fntkcjzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btbxenio.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3xbumdfdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pzzypxsl.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cwkczrni.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ifzoywxf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jprqpxif.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oetgdgsl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lgdervys.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3crbrokve.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hnbysagn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ggvrivfl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ggmetnyq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3isapcxyn.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3twkwzvvh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wvekehrl.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mzdcktqt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ujndbsye.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3iujwzezg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bcposixf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3giibzvsk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3yhjpsouo.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tifqxskw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3wyssrjid.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uvqrtkjh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zuvqlski.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qdsanldt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vxdugfaw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ffoxhatg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3pwpeqtlt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cilqbbtq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3erfwhilp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hnlubzrf.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3dokxwkvz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3fytpaxxi.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ilutfmko.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vqtrbawp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3wzlyzmaj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hgloqnnt.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vpmjnhzg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3tgofqpig.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kmitueaf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3eguybvmy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kydqzklg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tfxgyyfj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3aytujovt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3msaxjiei.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jugjmfoh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hyuuudgy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3sshvsyzj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dajmfbsl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lvjxxwjy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rluvmony.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lxnbbkmu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3abgmaena.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gsuumdiy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ihvrvdpo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xmhofabu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ddmkuwxp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3apxzhpha.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ummvjjxe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lmajbcmr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3xvtpumxx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dfuywaiu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3fzfwyulo.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3bnhsvlbo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3prwppvoj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3gjdwcpmp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3jwbekzyi.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3yvbqorrj.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3olfdbnex.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wowkwrpn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3tycyxsxl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3mhztsnhl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3iyqupkrr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rcyizpjp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3vnakjsvw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3iuuaikrr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3musfuaqh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ounqwfwt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pnmogpep.html


<!-- 参考信息 -->