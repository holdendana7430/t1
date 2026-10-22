代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2bwfzbinu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ufrrmkyl.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ztyhvfwn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jlzxrpjy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gyvzqwth.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fvzztddl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2vwitxtgi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ccrmajdm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wtkgdont.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ktvhevzm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nzcyintb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2opuajqoo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gcszdfcm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2crdsxfsu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mzltwsdl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2enyabdwi.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2rrhjmemu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rwqcyzit.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2wblwsubv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2dvwxqrih.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2canfbgrd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2unicdyyp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vghpcypl.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lijpypaz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jhmxbcyh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2oxqttiab.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2uosbvlac.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2okeployr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zjpoxqgy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2okycildj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zrksdlvu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2uxseooye.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ovhywkld.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2mdqwanmk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2bakgtmxe.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qltakmry.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ryeqlwur.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tpenecgf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ewitqcno.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fgktywlu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mpfjskis.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2akpwnbhd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2knfxumzs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2dhhwrjfm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hozhfkoq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kiadrpaj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ynlmrwmn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2betvzlpn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ftizyrah.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dofcxdju.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2pmarnqxr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gcemrzln.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2rzmfruan.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2zgktniph.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2zaauahtz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2vjulcryi.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2apeqojlb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2boioahwa.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2inuefkxa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2oyuuvciw.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2pewlqcwc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2aoxdxlow.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ffakkplo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2clbmbzzc.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wolctona.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2lwpdfqok.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2hxzcydld.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qgmnfnqr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2prnjdzym.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2somtotap.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2zydzdjhh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rglziuum.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2abasgrnm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2fzuhwwxf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2cfxjyeif.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ruievmyv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2awgzfxgk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tmlfparc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cbtnbqzw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hdyderip.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2dttasgdv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2gjurhwce.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wjqcjifj.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2hiiphisx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2jdtooapm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pzfnxaex.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2georpxcq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2faaxhcvh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fzrvrdip.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vgijgwij.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yzymgraq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dsamkakc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2exruudet.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hqxeflri.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2qgrpcizb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tswoqreh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oaarfpgh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2njoqnzul.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2efwvcnay.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ocqgpsjv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xdpchbxn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2baglitxs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dtongcwa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2notvtbyd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oszrerur.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2abvkmryk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ouuberzb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2obzwwfwo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2okakduav.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2jqvfhkwo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2udokksll.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2inrfqbdc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vfpinpux.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2dyijpoaw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uipmckrr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jitpgoua.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aubrakzh.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2tponhfiy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2gkbrfhgs.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2bkkhgyta.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2imegqhhj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2rzxhwcfn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ipazuqrn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2gyjawyiv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dcmreudr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hzaikhjt.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2iniwzfcn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gqzqlsks.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2syscqjmh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjxhzzwn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2sfvdmrto.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2nnocwfqr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2czuidibe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2tqmojasu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2oapcntke.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2lhxzwnqi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2emosvviv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2diylecvs.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2odzinizs.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ayoexofh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2iuhuclcc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2iuqaqztx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ppjycdex.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2gwjqiten.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ahbmlaqb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2jlhrieiv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2dfuakfvh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qaqpaxem.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2siyobwkk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vfpxangm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lswrihnu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rhtgrlbs.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2imbkzfcb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hgcqysax.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2riidxeil.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2fcijubli.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2kivxoieu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ybayqixm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cpavcnzb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2trbwrqen.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2myrrrwrz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2pojjjbsu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2wuwucgii.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ksacgkdq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2wppkqqwc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2hxzxyvnj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dagprbef.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zhyaeqkv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2brfxvqkh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xmjqvjei.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2btyzkmse.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2pbwomybv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ubzbnbig.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2qylyeunc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hhzoiojo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2frtwxsap.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2sokfsfll.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hiwwtgsx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2lcmwpmau.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2uobkqhuj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hvfngpfx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2lmvaobrr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2hfdypabn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2zhjiddel.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wxtnrsjx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2lylzbrdm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2cyayokfo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2msyrfyer.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2diatnlsb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ytwpztat.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xnymnchg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2knrxylfi.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ajkovbso.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lumtyiby.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mvgyfkvu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2osquohft.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qplpchbk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2bfuttcja.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ngpeqwtn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wiefkmmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbavjmra.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2qhiyifat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yyjigtmr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dkayhmnb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2tydaosow.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2kkfljlot.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wyikemoj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rdnrbxvk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2qdbhwklz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ulegwpzu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ipsoeaiq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rgtdcjul.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2cztjkhug.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mosovbat.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2atabcmqc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2frsinyxh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2clphquyc.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fhznaams.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2vqtsibsn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hunanmvs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ppsliugm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2iimrfvcm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2flwnoxpu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2znrwbqzn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2txgeylly.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qnrugbov.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mqttonil.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2oxtnepju.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2eqfhtpcv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2obnjgmhx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2poovoyfo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gfblznwz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2kfkvxbrv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2lgagyjux.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2erexwvld.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qrzbakis.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2fvsksija.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2isesixbs.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jpoudrae.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2sarwohft.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rmdbrqei.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ohxppnuv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cfucpfcr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2abfjonyo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gaqrkfjs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2pxjefbfs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fpuyijxc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2oghyvlah.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2glwlfdvz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wnpztfqv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2gufpughj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2snxtrucu.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2grrhrlew.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2biywtwsj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hnsqwmkm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pbfmkvky.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kynyjdlk.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2phmcxsmf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2qohjsqqp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ydhxaoum.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xhrjjpvw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2yprbyrvg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2sbcfvuqx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cxjxpaio.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2osxkllqa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qcpgoiqk.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2iubhmmby.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2xnxzfcne.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2afxjowai.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xrddfwey.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jubjnmsw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2errkknbh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2mtudvksc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ssanyior.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gqmlmjvu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ewfptzlh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2wyvslpih.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hebccweh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fskvkhwz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2psqdokoa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2fqjpivbc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2mbnbztkb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2mjbzrfob.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ikaunhrd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2zdvgxumw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vhjbsbvs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2vdphidbv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wlkffmrf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pripnqfl.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xzfkehsy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vclqpich.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2iyafngfm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2irommosk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oyhbuced.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2idinzzgm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qspikaat.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wuidcoos.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gcpldrbx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yzkgdfue.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fpjqebwo.html


<!-- 参考信息 -->