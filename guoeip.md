代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2okeqkcip.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2psdpsrne.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2adnnnhzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmpqnbeo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2hwuwjgrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lalsvhyx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2frcstqnd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2aadwnkmj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lolfxsut.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wqutybpe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2spwplqoe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2wlybatie.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2xnrafymd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2prwhoafv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2nipjxbdj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2jtrebcoo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ratneknq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2nuditecj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2blnhcigb.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tkgdufry.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2dxgnxsci.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2zztfszad.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2jrzbayrr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fszscmkf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2gvvsyzid.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2sdooqtay.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2bjwiajfq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2gjrsogvd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2aoxiawmf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zzrglcru.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2bctkzrad.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2cxuvsvmd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lqcoxkwx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hetxjous.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2adqoudle.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ktbreugm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qfwboijn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2gbizbzdo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ukmzmlmn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2iynqldpa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bheolwas.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2hujdnajv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2eplttxwa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nzwnahpe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vmrdtawr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2osxwmkpi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2sdjrlajl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2gugbfthz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2npxjclgb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xgnjipuv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wedradkc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2evzimlyi.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oqqdsfzy.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lgaheukm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mwijhryf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2eekiythr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2jatflmis.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qwgfzldt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2jgygsldl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2jcarxzuk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2nbmpzluu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2elgpdiqv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dlfdwtxm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fzdogfqr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xkpqiojm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ouwfjcwv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2orgrypps.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2moxazopb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ltxorgel.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2kueihevd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ydijkfzc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2rlbgqkjv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ethypuel.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ksgevoxz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ackwiksf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2mlzegepl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dlzuuper.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oqjjtccz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2decrasjb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2arcsqckf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2iqfjwhjd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2hoxccihf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2alcewdud.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ueckbzlz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yhsperey.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yxmwskin.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2kmqrhpmv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2sruivsev.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2cybqaykj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ydxwbnwx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2oahvdcdw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2iwdywqto.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2yzdtisst.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xfcaqqag.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kfpemayl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2shzzyeqa.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2urfwiqqq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2udhuhuab.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2kirbgyrx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2otxvfxhq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xrnywkow.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2idupmrvq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2caqobzjg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rfxeijli.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bxlsldsr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2idkfvfvl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2amlunska.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yychicmy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qcytaqpo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bxxlxtan.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2pupnrklx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vdwaxbqo.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wgowpdpj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2uvsfhhyx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2pycaotvj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2vmoypjfc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2jojohyxh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gbejrfzg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iuqutejf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ismgympn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2fomhasrm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2thjhvoih.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zbluatiu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2bceaahhg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jsklkxij.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2diwvclog.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wctbthvi.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gvvbxvxn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rhqjkxhi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2eyaxblnr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kowogmiq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rjzqwayv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2utjycryd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2prauqnpw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ucmlqfxf.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2chhybsws.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mvspgeqe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2fedpklnp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ehpgkxkv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2lufrwgkf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2fmyagnju.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ypddeocq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2horzwutg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fjebkidv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pmefdmxp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2biskprbv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2pbqlmzqf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2sdluulfv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2brnorgnd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2pndyoguz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2saqgujtp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qubndevr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xxcawjuc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rejjkieq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2roztnljj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2xyeswfig.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yojpqmvu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2btkyaykk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2vwpzpwcb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2odrvobyl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2jwmjwowa.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2xwrlyuyb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2hdyrlvpo.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ugpanybu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ggpquyzw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2todilyzg.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2zyannmon.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qgqjhdia.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2szjvoppw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iixthtvj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2byanlmbc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2dunjwidk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2pkdutnwl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ljbzkcbi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2onuyewcv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2jtfcdmfe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2inatmjrd.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pnkupyrn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2qipqvzqb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yxeoixit.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2sztaczhz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2aawoefuy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2pvlhcnfm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2dmoiycmj.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2mwaozwbs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2revlibbk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2chebujtv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2fsxttkno.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pilbxcav.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wfnigalz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gsvpwfvt.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bfiwjxdb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wflytufu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gfqtuiln.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vrqduzyr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2rbfontdw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xewusxdb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2usxdiyjp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yhhztmtl.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2iagrkbyh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2hdltmvqs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ncgadmbe.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2xvqqksvp.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dtstiuau.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2uxdiqcxh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qcaaibkr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2lhxnrhdq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2djygqhli.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xsjefoex.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2vqjoddij.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dzkncrqi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2kxggtleh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2xvndgnaz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2pxddxezx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ghddfyqi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2mnovguxp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xpbgfjrl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jielyadr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2gmocexzx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2zbaekzyn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ynbrsayn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2vtetvanb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2uelmqisf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zghjdvfn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2tqxghlbl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yqelbuxb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2nohfbxdm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ezxuqznu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2hsxildav.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2avmlgwkd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eorcvssx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2dssclkds.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2yaovcpcz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2webqlqwj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lwivfxmq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2epaciugw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2biptednt.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2hzvercdb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2cyrhuaoe.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2aucocfju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wpilyumy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2euhgiank.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owilpjop.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rjfgftin.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2mgdxznop.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tbpxxeom.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dsfyaqmb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ojpfmeec.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xoczdblz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fnxjagit.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mnhtjrbu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2stnzvifz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ftvcusdy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qbniczrc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2cwogyyvz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ksahfdxu.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qelkqoyf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2idjwowim.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xrazkyvy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2udnyzvdm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2hetmecjv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2myanmopj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2bazcfsri.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zvghkuim.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bnemkejt.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lfqujzvj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lruuyztp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2uxfiixot.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2kmzrqipx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sownpqas.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2fxhgiahj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qdsuiqxn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2cxxkaepu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2lfznqgct.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ffjzbasr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cvoscrvs.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2dyheeqlq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dkxyiqlc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wlatggwf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2rdcpylxk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lmwgpmlh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2dimuhvou.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nbfclmos.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aftclxys.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ofpobukm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2khphtokw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2upupuehf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xboleqmc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2gezyknmq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zaftztsd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2yjnuzexv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uikqsawn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dlacolje.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cpdlrysz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wcikxiox.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2anambxjn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rymweyea.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cedkikoh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2lpkbguxt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nrhozphg.html


<!-- 参考信息 -->