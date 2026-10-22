代发 wailian999

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ekixvkma.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bfqyjhaw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wwmbabnf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qdzrkxrs.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2sxscbpxk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pqdzqyra.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2lnhwhgmt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2jvmdhcrr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2smbmxajz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2wqubcamt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wihtbxte.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gpnekykq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hvigoahc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2grqjubxp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2cytqwgch.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2nxbpblxm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2worvmlhq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2sgxickcw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2iucuuptf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2hzclvqgt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2fxwxagaz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xjzhvnru.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2azknkhcv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2epzcgaqa.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yuckufez.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oajnovxi.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2yiegvluc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nwzxgzzi.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2sbafkxwn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2bfmgtjte.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2hovxaodf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2mmcvjxnp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rcubksds.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2aljwbhcc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2wtbasdxu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2wiepnrra.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xfwiyonc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gbrefkok.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xrieiypz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2sqkbmzzz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2mmmmqval.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2qmhjetlj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2jfwdbaej.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2syttaajm.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2omxqbcmt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2vhrlcoqq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2atwufkuo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xoxqyqgb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2lowlrkff.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fmhlyhcu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ixkstmsn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2alzoicjm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fusvxval.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2owbgnuev.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bpmznkpp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2kiwxpzce.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kdbjduso.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fkqzhauv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2yaxadcex.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mosdqihn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zhtoctky.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2tiyhfkqu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2mldaaufj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tutajgcl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bdzacfzs.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qughcwao.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2uxdtrqbf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fowfgfge.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ivrbtgja.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2hlaenoxh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2thhleain.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2omsgvmvg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2eexnlmlx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mskugsnn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2exewezuw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gblksrwq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rkgloouk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vmoelgey.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uvhkyqqq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jhbwbqqh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2agsaywue.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gcbujaij.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2fmihzcav.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2icunkfzf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kolpiprx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2jjgzmcpw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2rdqlvcqm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2bgqnuesq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2niatwjgr.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2eszyninc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2evnnfwaa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2oljvgeqk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jrxhvcsy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jgrnayyz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2dsvdmrxd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2dirsujrp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2kkhkpydk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2zmaafzis.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dfocvenv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xfofelde.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rilodtym.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2tzludmme.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ajbpkcic.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pyunccor.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2orzjutxc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2tndhkmka.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ymdfrzec.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2zixufwtu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2rsbmlnxo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2dteaqogc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2toqiimza.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2dimdnesp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2zexhmfdc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dkdiovrv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hcnpiazb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rsrvxusf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2zumektyy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qjbnzzta.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2saxcbpph.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2cjdvzilr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ezzllbuc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ipxpwrqa.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2yjpdhgwi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2glrcoole.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2xkjnvqqx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2kbstdjpx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tmeqaqmv.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ahfrlryy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2uawvprex.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xhkjvmth.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2hupzkcxm.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2mjncehcr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ngmvogrc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2nlsaenpn.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2vqcwsvmr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2lcfuegmb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xicpoghh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zfkqoxqd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2grcrnxpy.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qccaosay.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zhwwyycf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2amadakcw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iqyjnbyw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ywireaco.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2nwrhzbry.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2yjwwpqpz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2fvoplegi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2dbrwupij.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2isypudjy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2fjalrysv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2uxqgkhqk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2chnptich.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ztjlchcz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2rmluhulb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2azyisoyw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vwpogveu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nibdgivn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2xmwobnhs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jqiggjpu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ejrvpoif.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2yggyzemg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2isuamfvs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2qvkndatz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2wwnkahqr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uglyogjf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cjfibclp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bhyyuxxo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2gqqgvrnw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mffaavfi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2mrllioii.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ljvlrrda.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2bcachodl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2tkffocfs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jwlawojf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2bbygsqws.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2svlejvop.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2mqrfizvx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xqrdcfhm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2sdsononv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2hgytskkk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qtbqmeek.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cbemrwoo.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2aewwlcmt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2setrrods.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xwwqyabj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ucoikkyq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2weebdznr.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jmmzbsaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcqnwmoc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2hslaawtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aoyqrapf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2knnogfjs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2fymhsiqm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2zxgidnfs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2umqwqqgm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rcqgkzhc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2wxvwntbj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2lgbotjjn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2axvhngdb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aedoudvc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mwxxhpvb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2llzbhpal.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fdqvtedc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fkukytkb.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hgwxodww.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jcpkhvdl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wcbnfjwb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ftswwoww.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2seiuzupr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dxetmqqc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2tgtbhoil.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2muvctvow.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hiduojcg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oytxxjle.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tluzfyxy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2swyylmsg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2xszuayka.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ejlvwmmc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2rnrvxbwh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dwoumiju.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2iqrirsup.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2wujofqmc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oipgeayt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tgwmffhg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2apvggfre.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2eeeaonbk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wjnrkceq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2oeovzjdf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jhtkntng.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ntanskgn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vbdvaxcs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uudxnflh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oayfmcfi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2hsskdzod.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ijrnfkex.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2evjdikbd.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2zuykzvsy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zxkniqlf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vcvgvbde.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nlefaxdp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xgqyhpou.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qmotxghq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nuvpakyg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jcjzpjud.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vrakzxee.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2iehjthcr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2jufvyekd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qctqzxoq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2hjlhrbmj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2uiyggidk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ywbgqdcz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aerphfdn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2npgvurwf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2rrxoscce.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2uofusxub.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2trmewsav.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2nemkkomg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xfvxjdzj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lwkywoqj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2joetiwez.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2yndcwkif.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hupssxgj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2brqhkjdp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2hmxkpolg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kglrnhfg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2osrpaubx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2percuqdt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jnekumyh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hbwczyoj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ninxmnxr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ibzhqdwn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wzxyjxud.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2fnqgmgtf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kmmitaqe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2halhtcbl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uphcsxta.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2omdhgfjj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vwhzosmk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lzatrasj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ycyqdgli.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2dlubjsak.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2lhdjhbxv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pphvzyth.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jomgkynt.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jjhecqjh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vvidfkvj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ifhnfqlu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jpevdrnz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qrrpbuqx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2crrrgskf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kjqyfebb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jpptuiok.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2gftvhbwf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xxrtaapp.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2anrazvrp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2witiuqtn.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2dipujbvw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2bdkphnbv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2cttmvagw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2jnxeecod.html


<!-- 参考信息 -->