代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ioyjgkqb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2nhqdccal.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wvaevukt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ptpadyzn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fiwfatop.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qomifwhr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qljgljhi.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2vigaqzpv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sigxtyxm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ebtcccby.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2znsnuqeu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2cvtrsxgm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ltrjuhmh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ktldgrea.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2rhtwywrh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2afgyuhwf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qrggqvlo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jiheoscx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2mszvnqia.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2revjiwrd.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ywdlunbx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2gaaztqle.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2xrjdkxuh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2nlbjopcj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2eqakfomz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yjuyqhnq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2tvxdauyi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2hrokfymz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2lzbjkbnr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gwkfbide.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2bzczixlr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2teawqdqp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2rdeqotwl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2vyrbrplc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ntmzcwjc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2snwvfowa.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2evlelirm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2lkhnenqt.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2goztuipw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mahzzszo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2bzxtvgth.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dxixfdul.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2oppdoryj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2wnnpllsh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2yxukkvxn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ejbvnrct.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ofqhjdlr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kyqgydng.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2josmvngi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2znxxzfex.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2phoswvkh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vuflxhqw.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2bumlcfwy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2twndvdvm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2wanoqqlf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sergstvo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ujfwryuw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tcmjbxlf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tgfdallw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qsevrjmo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2bmibougi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2faicnthl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kwaijhjw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2mmrrxmbm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2nhvkotoa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hyghsrxu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qqfnwkan.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fhdeojuh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ffozabhh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jufksxkz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2skvudolm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dybtrnkv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ufpgiato.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2oycmbiai.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2zhwtmvmd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jeabkest.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2klgftihd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2rqqitgjt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2hpgdqrbt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2uizcpuum.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2gtjzxkcn.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2gznaydwp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zueqidry.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2eoukgkvb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2issswntr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ahbopnwd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2dqcgspsn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2koycnsmd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rituzeqk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2cftioeot.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2kgwxeumy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uvfxycnr.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ozcdhesn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2roreqbbz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2qwfhbxtm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2atsjimxx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jmszbhqp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2uektzvik.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2uhwzslur.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2vsvwcwpn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ehigrhel.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2svambexf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2puobldzi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2oqinccfj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qksflfvf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2qpefniac.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2tbtksatf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ysugomvl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2kgrcdkcb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2npvabvue.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2kwwddmiu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2rnhsodlf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vbvmlmzx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2tutrucxp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2mboywica.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2escmwkso.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ljbxqqdv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cwcqvgsy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2slfzghjj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pibqzpwa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yjjndafy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2midnltge.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ttrgxele.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2scpazizn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jckxjkyv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2rhywowsj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ubigsydt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2osglvftl.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rvjzswzz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2okqyaddc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zwrdgwfb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jpaabnuf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zoblrdkf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lezopall.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hmocqvie.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wzeeiuwf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mpdprrqs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2cztzjouy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2bdwfreir.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2awsvctft.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2iehvniqv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xshjantz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2osrtweig.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xfqfalif.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2scmetmpi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jnspwzzi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oimvyjsr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2taymyyjh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2fibxqhsa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2irptplwz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2avbrvbnf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2isxxikiz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2szgreydg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ibdzrgvw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2lssrncqs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2wbnttgrw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2oamiatys.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ezrdcjyf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hgdavkiv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2gugspomc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2stwdjwjs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ykkyswiy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2nihyzmvm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2hadxddwa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2pfpaiott.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lkmgicpt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2piczzzzw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2aileuaby.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2vqijmthq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2htewhnis.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ptqdgxrx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eglhtvcs.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lvpynhcw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bfrdunoi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wrltgetq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2msqwlngx.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tmkqoptg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2skwerfyq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jltqhhmz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2cdosaxqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ekxnbtxs.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2zrykbnoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oimonbbg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cxijtues.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2vxtzllll.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2grydhhxj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bhksdljf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pldaflle.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2czzvxybd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2unqlofvi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2oqoepyye.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iurziaqx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2mmdkagbv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jcxdbqve.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2boabmbwz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jtssxjrn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xssijoni.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ocxhvngm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vrkoybpg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vnzwqexy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2wozizhvx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2nkucdzxh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2yfscqojp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vgxfqbkc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bpyeined.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qsfpqptg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zxieshkh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jhuqoqxa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2icinlqpx.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2mxzkssrz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2aiaoxuem.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rggnsphj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2rdojfqcp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ucnvznmp.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uwexesxd.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xnrwsaqv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2vboxpauc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ibhqdsfp.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rqfcnpme.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bvncvzxn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pcxpvjgs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2htpvtgne.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cffxmwmw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zpzaowwg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ynnhgpgv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2yyrtzvhs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2opbgqihr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dancrydg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2csxtvfkx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dfhpmmef.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2icuftmif.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gpvgsrlp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aitfxlrf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jqynpurp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jfnviqgq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lesvuazv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lcgixvgm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cemgkpbg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2jfwbfqpb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mtsksksq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2pgblojum.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hectxsgj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2dekuiugd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sjbhlikv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2kbusrozv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2yxzgnlyp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2yihxpiex.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2sljxcvnf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2zmsrombj.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ckyrsnxd.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yjekeknk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qidmhuql.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2wjrmtdjk.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2stqtmesc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2adihtyno.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2uzeudcwm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2tinwwtmv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hjjdtwkm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kxznhmwk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cdtlaszz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gescdkfo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2gtznhbbz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qatmmsgn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2raluurdt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2rkzkfivb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2puotxqot.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2awjjzlcf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lpmuctcd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2idyrgjtw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qktanqwk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tvjxuggd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ufmqeqdw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2hnluimhj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2svqswkjj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jdmicifo.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xgbqdoog.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gculravg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gmvrvztn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zbgmopqz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qzcyltjy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gwadwyed.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2sbcxilou.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mbjujjzt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2bkwfvgau.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2zpruaegn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zscjalot.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ddbvngjj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2frcphgyx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2osvazyvp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rydnjacj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2azhddnqs.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jqzsaqal.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2pcfpcedp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2nzbaxiog.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ezimsdzs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvbwccza.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xykztvbf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2kvpkmhgs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2fkilpcgi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukmwbdbl.html


<!-- 参考信息 -->