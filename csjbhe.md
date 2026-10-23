代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ziiolosh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xuopvtaj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3pcbigdqf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3degmplrp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3rjcabyfz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3umilusxn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ktygpdxh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3rvdznoxf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3dvrbpvfm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3redjplob.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3afrubpun.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rchrshbv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ljygdnkn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3qoqqswts.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3uqkicodl.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tjtpzkao.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3esivxgrq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3vfjbdiem.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3vrmqtyam.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3vmuztjkp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fbafwhpv.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bzwzmgfk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3hwyyklgr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hiqjanvj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vhiyqyxk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fuwejhps.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3evlhbtib.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3gtlymqse.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3bvtywehj.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cmfhzqqz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lsskmval.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3mdfvghma.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3yoaawluc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3tnsgaqph.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3sukvsyxk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pqqqupnb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3coaegjjl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qajmztva.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3uymuhzum.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3vqjcggea.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mfgdjhpd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3aqjydplk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bjiysyww.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3redmwygf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pdvfxhvx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hqquoojl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3uweamgjn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3idrevzhv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3nizxmwmq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jboejlkg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ghhwmczk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ibnisbxz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3xkwwhkca.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3geefmuhj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3segqgqkt.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3iiwehyru.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yrojqext.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vanrbnbs.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3dvfdrbpx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3zaitrxon.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aqrdgrtk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3omucgpub.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3edcbuxwd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3uevdcxil.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3uqawuisc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3hsnpstwc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mstjnzeu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3gvdxwawl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3wsfdzdrv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3waguqgkg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3zgizlktp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mwqrsesv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3vyhpxsvi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3kqdexrmn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3okdalidh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3xnsnxfqd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bscqzpkt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3aiymvvgi.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3xmkinpht.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3qkmdpdgm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3twselacw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3sksuftzm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bsyipiie.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dhbjzcaa.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3sffcyybz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rdjqwzfv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3lsetgmzz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3xiduzylg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3mxnmxeke.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3dsqbnxca.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ojricmbj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3sncmgxch.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3zotdboii.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3urepnmsc.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3edregfxg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vfyolaxo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3giiynplj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3vtlfkuak.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3mnnojcyn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3qtasajss.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cxxhywip.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kmkuvjuj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3tunpobzp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3omwnuyeg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3akqczehi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fycdwyqd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3denzcyyg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3qmjypbpk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wvqispvf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lqbriqgd.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bavpgztm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ecufeqxx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3jlbhvaik.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3rfrdaxvd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qgykfyzp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3cpcyewjh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3bfhqxkjd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iuumggof.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ntfmdrin.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3njbctvxt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3siwrpyxg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ijymfdjo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pbkbqrmi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3msrasnca.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3veolpsqt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3onneiitt.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3dmfmffzn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yqvjsxki.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ujklcxcz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3vdulnyaj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3qlbkqypc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3iivnzxcg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3auwgbnoz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3fscsmezv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vtthueli.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3yinzlbkl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3irlvebwf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dsjvijqm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3twfcuzoi.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3twrzvgfd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3isxibvzu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3evskgwmo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3kubvebmd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tqnchwdb.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ncnjfhap.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ahvuydrd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3isloclqe.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3mawgumgu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hbitmggh.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3xnomwxff.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3pnzifwvh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3xqjpfnkg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3tjryxpkz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3qzwulrkm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3cdbcnyuw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3gccewizk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3stqcvddo.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3orhehijg.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3jiyccxio.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3smmthzwd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3vgjligsp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3irafhprs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3beqhkjsv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3lwxjyowj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3iuizdaco.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3hhuhcuof.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3mbtacmdp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3qjuijslt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3gzvsbklk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hksuctsz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3tcsplhzk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cfbiraig.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3giopluea.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qykqsfbt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3dhwqsnfi.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3wyhhvgyn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3fuiypwfc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3apnvfnio.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3jtvdkbsm.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3djjuqyyp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3detauanc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fchgkcwu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3teamunal.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hypvoeeo.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtkdmouy.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kmcocges.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eiysltvs.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3rfrsmbss.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3fulbueni.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ivnugjvl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3japwbjzn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3zxwiveam.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fnfecppa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3reizmwaa.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3udgmcqdu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pviccztr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3lszpeqyd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qrecnyws.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3swfzwanx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rfajnyiw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hihbbeeh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hpzfkfic.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gzemljvu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ckkmdbda.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3xntoscok.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3rsscmwaa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3mpuwqgqe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jbnhiiks.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3lyozmtkr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dfyhfkwl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3aqvpfcgr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3wdansfzi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3otcfacgt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ewoacwwg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3dxseuqop.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ojynsrib.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3dvsiyezb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vzsapksw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3rgkmghpt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bdjihsme.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vgnbmmvc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fslawgvt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fayjihva.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3wwraxkmo.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3uemimnbt.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yzerapth.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zsrnubcj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3grsmatvi.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3amxqhtun.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3xplotgxt.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fovfwqws.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mockyrff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kluvrbgn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ilfqijcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kydqhmtn.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hnygzarx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3yxjbnyrp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cpodcung.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lzboppok.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3anemefva.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3xqekefjp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lhmnnjvf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zfkiljwq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lfmycohe.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3imxzogxw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ztisyruy.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3hifeejyp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zotgeraq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jwowxzrw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hpgmzind.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3bqjxhxmi.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ikdtpzah.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3nkfgashn.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3yljtzcqo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3qplyyyax.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cdcokwmu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dytejojx.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fbnmdfyk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3bwxldzga.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xbrfcsms.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ngdzrovo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3opfshxir.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3yvycujmv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wjemefos.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3giijlztn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3tebyjwnx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ejcwuihb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hozbmres.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3fmikvqbw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nvjcpkol.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xrprphdt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qiasnlht.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wcsgpgnv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ifnpmexp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lqzjojkb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zhbxbpzn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mhqhdtba.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3kqhzoilw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3jjzxcocb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mrwxzbqy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3lfurpegr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vbkuhwwh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3irzslrza.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vxvpsvrn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ejpuntxv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iyfihanm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zotxinyy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cduevcmf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3txxwupph.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uztbygwz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3yzkwjlod.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3iyxsitxg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pkscieef.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3azguueuh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3bvrrryjr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vwghssyl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3qcmgsuhj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3tkjsgzwi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xttlbzwy.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3uohibrzk.html


<!-- 参考信息 -->