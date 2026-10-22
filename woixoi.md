代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kykfvdns.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kkiquysu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2uryxwrds.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2xqiftkik.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2fkwstbmy.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gwqhwvsm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ruziosfl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2qhuqnwxh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2hmnzfvia.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2sdjjnzud.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2losccdbu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2frtdooct.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2skbcigiw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fdbnwtmr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2gibhhkjo.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2crzoqzzc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2bqkfxncf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iodfvsra.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2yymjcwrg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2entkdcjh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2znjubmvz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bgwgclgp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2oxoltgzi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2hapuxuvu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2edldnvnc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vfbowqvb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2okurjcno.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pcqefoby.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2vuwapkgr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2kmismomn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hxskmcbz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2uwkzzoba.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ynilalsr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2fanybiuq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2yctfgbby.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2juzbzpyj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tqlfbuah.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pbciomja.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2uzkdmsga.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2frpvxkrp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hxdxahsb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2umdxzayd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2quylaltg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cfimcxji.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uxuxqife.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rohegtwp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2huioerkh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2symaorbd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2spoukkru.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bcklnsgm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2wsygqwss.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2eufvejmx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2zvnzlsvf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2dvqlgkjy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gfrgnzcu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kjakvawx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2chyogbmq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cgnzvktm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ijqctkxu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2llpcqbmc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oqgtkggv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2kohzmmgj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ffitfyok.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2eficsemc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ctxjdbjm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2akjojeff.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2jyozdwtw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2jrochaph.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2xutygodk.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iagezhaz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2xeialhsm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qbgwfccx.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2exrrsvnv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2wsunfvkl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2gsvxjeso.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ncoumxng.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2twkrcsxi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xvxsqgnz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2pkzeooyp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2hvrykcep.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dffgjsrp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zlkggqvy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2yzvycgub.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2bdzjufmv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2wvtlwtra.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2vbuvfmux.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2cvkfavug.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2rygiafrc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2jzffwmmb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2tylsbwct.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2tmrjuulb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2qhvtkkoe.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tnxkwwhi.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lhdhjnln.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2jgltzxzu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nrphepyu.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2euajvwbi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2zfzlhnrh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ocmdydwg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jhsztxml.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bqbjuqhf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dgrgvcqh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2zehzwlmr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pqoqxpyn.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2fxyxyfqt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2rfqbsbux.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2sjijhynm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dxowjsxk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2azpfdcnh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cpoyochv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lniydezm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2slwmygsn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2osyehknn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ggeueleo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eayeglii.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2zagmwbbb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vzntojfg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lcstiwus.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2garoqqbt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dsxzthcm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uycfwqld.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2traxlmfu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oqbocacn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kvrqmdxn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2tglfkeft.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bbahatth.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eelcmdbk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fdabwhak.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ugmzzkxb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2pcqukpwq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2jrzvxvkh.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2lrwwupvh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2clfbowdw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2hbzpgoip.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2apncuuta.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ejpxltak.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ppxuynvo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2myycphez.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2qelqvbzw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2dlxelxbz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qozvvofa.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2mmwqyanq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2wsrivyae.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2msjwhxxn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cadkjtyb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2grexjprx.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vvalxroj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tysptipt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2sbzonxbj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2qxlywwfs.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2kmgelafa.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2fpvomwfk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2dbldcpzc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2arponstv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zrfftuqv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ptwpedwm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2evfbzivs.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2eyzxvrny.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2nhuhvfrc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pbweniem.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2pxgbxuzn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bkxmiude.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2xvoteeyo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2hjbybfne.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hajolykn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2krqjwfkt.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2otosnnfc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2mgztiajf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2iipaqhik.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2gtbvsznv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2kwlayqyk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2kegahwpg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ncpardzr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pgvrwwpb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2connseir.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2eqnqkovb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2edcbyrrr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2gaqkmjis.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2tvviuzhj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2buzfudfy.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nknjgtiw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aflzywrk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kgzprwoi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wimjktti.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rbhyjqcy.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gaphzwbt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ieivxkvk.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ruxufaud.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pgszoiaa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2bprodmik.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jecmirvw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2efkmrohi.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2pktcyetc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2beynernq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2jldujqxz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ioftznbs.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2akvxndqx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ghuqvczu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dnuulxwa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ckqpdwyt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qtsmhirw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2velovzmo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qpmeteoe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2gpgbesvm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ernbowdy.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2cegeokdz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2tbpbjlzb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xdccvilr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2gpqoajoi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uzzljiwm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2xrejsvjv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2bevklnyj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dochxkke.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2vzxovgyw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2yxejtyxf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2dxrpacnz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2whfekdjt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dunlfpeq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xkhomvaz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qhgwhyam.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2erwtfhbf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2tvlbifwn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mavtddkw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2htqvanij.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tyiumrkh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ikuellgm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dcfsxdfr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fkbxqjcu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2eofsptiz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2eshwylnz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hyqllzzg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qezwrujl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wyepkold.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2hcjfzeut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpirzyjw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2unmhirha.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2nhwxieit.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2glqlptmn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xmizookp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qxgkoefo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2bvbtyjte.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2umbctmgq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2dyghjuyk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2swigqwqs.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2mtagnuqg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ssztzthd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2mfbzqilv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dyuzcvzn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2iunevbdv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mcucovqf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2fkfsulsl.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2gczfqfvf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2fqiffafp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2szqvdrlk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2cwugzynz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dacsdihj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wgwbsdbu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vwmpgfmd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gcohjhcs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2nocgypqq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2gxrtgveq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ekijqdtv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ripxtxhc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qqurviol.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2hdddfrmv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2fyhpvivi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kcktgxul.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2twbpgxjs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ialfsjjv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pcjsmobz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gqephjvi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2wervbsft.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2soxldbec.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2nxtcptnc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vzmhsizd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2elroxqcg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qgnzfjkb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2fferdekp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pdpurwzn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vqokmyfm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2woklgnce.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bsebpbpu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bedlehec.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gyrqsupe.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2olbochgr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jhasqpet.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yqpxihnh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oudzcjng.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ftwabhda.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2eyycjhod.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2qseeshrj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nuuxaaft.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xzfcleyu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hkcdyuev.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2vllqxsjt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ialykvnu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2gkoadaip.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2dtpdhqwp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2qnywierw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2buyptwan.html


<!-- 参考信息 -->