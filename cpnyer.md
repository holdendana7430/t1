代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2oebzbgon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lgtqjnbe.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kpmfdwdo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2myokoxjk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ncswaoji.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ujztchio.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2fxkfhfmh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2fhrjorok.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2mzqfiilj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2wrfbefxb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2lovmdzhi.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2jljmhqly.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2gzpplxin.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qtonihsi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2oxsykvby.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rqeosnsw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2tlfqurjg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2enytytsn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2gydnmfwa.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2fddagadd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2vqzsdzfz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qlohwnhh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ankyxzta.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2dkvtlzbr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xrsgcedn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gvsswupf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jeuahdja.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ohxbvjwo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jxgjarcm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2uzqncflj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2hohqcnnn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nfmjhbbx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2jstodoze.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2patnlidt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ylzhuqoo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2znevpxpp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hfujdlsx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ehodlmcj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2mojktybv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vbzxktwo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2klsouwdo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2edfihnwj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2byjvqxir.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2azdbuggb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2curagcob.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nycsmqeu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nuuyubtd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2nvgcbihw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nllceaog.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dqqzbjjo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2odlccuun.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2sfhjspfj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2fmirrmok.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xfremkrz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2gjtflwly.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2hnrggiet.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2exlmmpic.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rczjqofz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cqrlltkv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wsaaqhbn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jjzmugtj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dusesvcy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2awwsitym.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2dzabnzsk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xxlfapxj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2yubeyhxo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fvnzpuau.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2zgikdsjw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ujkfvxon.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2lozsqwli.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oscxzpfh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2tmwylpbn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2fchpapgq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fonhpxud.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2mjztcuhu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bqhlramh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2vekdfwcx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2dfdobooa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2dyqcturo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2yyjcfchs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xlmbtnuz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2oacwirve.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2gwkcpggn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ntpcraik.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eqcrmuch.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qdosdgsg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tkrxyioi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ebztuspu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2xivirpvm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2pczrirkj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2sllbymmz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2wzcurdwk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2mjhylixk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2nltukiqt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xybkvdrd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2rzcgvtzs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ochemrku.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vcjyboix.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2icxxgwja.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sngjvtre.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2juhuqkud.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2gflixuke.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xpwkkerb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gzpstnpm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fmleewjy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2smpxcwxb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2grnjxbpj.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2quejputa.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2jhyrrsyj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2umotyync.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2nprnvrna.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2fcjbsngc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rssfxuqf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ypecdabh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tyvnzeaw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2kktgbuwz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2azvdaloz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2uktmfllb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2epqvxogq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2sgwpodwv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2abchtywh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2urzcumts.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2twulxqit.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qynvvkca.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aphtwzqt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qeqbuwfj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yksgbnki.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hzrtqivn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hwkquanw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vmbmiaib.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cswsckjb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mmiovzel.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jomtfxfa.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2polyluvb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2rhwwrbgw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ertlpxok.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tuhhxlac.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2bawgrskr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gesljamv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2biynnshp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2javoyqop.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pdvevczy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2yuuygvnt.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2djqwqaew.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2bsgnqftn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2lbwamkkj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2sghlztun.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pezlrklj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rmeyaean.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2aypayjwm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ywfqhhqg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2fjlixmho.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sfbkydly.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2gcgoehtb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2rdcsuoyc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ziudfaus.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2zdbklger.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2nvbweawy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2iosdoqap.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2adqujizv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2iybdunuf.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hazrfsnz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2vjzxwwlf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bmhspixl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2gmtlqinq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oxpttxeb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2zobtwwap.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2jlamsfzl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lvnyxnta.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2nllfgzun.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2tmdejodv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2sqrmdbqt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2kxwfaxsa.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hltwrmta.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ensrzert.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ilhhmbwb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ivhgecln.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2aetjfszo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ptpyryog.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2cuyblowj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2kvzvfjwt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2fvdngery.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2cduffaxw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ahqulbvn.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ajsejkzk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ioniryam.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2znnjlaio.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bfhmxgzd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gxcanazk.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2iwsgfcql.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mfadwsjm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2alipapvm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2lteijrvh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2efaxivhl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2abligtid.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2qncwnygu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2crcggxzn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2jdifvbts.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2cefjeqji.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2mqbmidil.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ljrmalbe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2lrvppipf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ibuhxrjk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pevdvznc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2exfetrvo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tjjvcncn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bphyhtur.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2pqxgdmmk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2jzgnqccg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2uffknqwg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2hszlpzvg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2eoeidtls.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2mmvwlbkc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rdnsoxvp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ehqmmupw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2cdtwfmco.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2xtatpjxi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2goopocjx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2chesqbwx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2xrcscizw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2viwgzfqn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jqatbgub.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2gkmqvmyd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iublerbc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2caruzerw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xjszepuj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cdghzqfd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2esvpseac.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2wewyamlg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fzpjjaei.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kuvvblab.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2upufgrku.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2foxrsoji.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qzyecsks.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vavzsuzv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gmydhjum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohswbrsg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2mjiolezq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdmcnhcr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nwrbqzhu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2sgjigurb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2feizlsov.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ocphhnai.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fkxgboeg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2sjwyyvwh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2omfkqwuh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2tjaazikm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2orbwcing.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2sqltopjr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mdpstwme.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2skbdipwp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2thsgtssy.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2igsabcqi.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rexwvbka.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cwxduwjm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2znoxkaam.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cymuqlcv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bqtrwrah.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ejfifnnz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2medwpagd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hmznimcq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jtfwcrna.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2andrtxnh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2mfwhurwa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2torxemyv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ijmcesva.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2wjhrwxqk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ztxxayqa.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2uqhiktas.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2zuouidsa.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pinrwoop.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lwmrewjj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2xpwldsey.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2awkhjeeu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jkgsgvza.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2dseuhwxi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ajfgdfsf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2tjsxfpva.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2csmirhiv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qejvuvba.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2eajqhsvf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2vqxujwrh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2spvpycgh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xiltjold.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2rhloptfi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ffollptn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2unrexyid.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bdtlzcqn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nonfhbpx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jnapiljh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2shwkugbp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zrwoaqvm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2arqppvbs.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2nmzpfooe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2slcnyunx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2izllolav.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ghxmnlwq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nvqjwthe.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2qmovhgix.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mukrhfhd.html


<!-- 参考信息 -->