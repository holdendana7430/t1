代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2tcazuerr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ufgckmtt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ftwexjkd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2kvxxoszq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cbgmebmb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hjlgpece.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2dwylmckn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2utyqpuko.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2bqaqqenh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2kcwahzck.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ewcxptyc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2slxbdvol.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vkudlbkd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2sqyjmscv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2xpnsjnrb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2khhjmxio.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jxlvxujx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cifsleqd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rorxkjir.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2pycgjbcr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2uhyrgfyy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2woklgtqp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2asxpuwso.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2mvptdfci.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2xajzhdad.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ysjflfbn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dugeutae.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2hbwgmwqt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ejnypmcv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mqwsriox.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2bjdzovbn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2cvwmkhhk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2wynsiutw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2gbscfcyb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2jqauptpm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2btpkibkr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kbjoavem.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2uztbwcbo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2aqxjbsse.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yqaihcvg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2nfxxscxq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2sjsjjqpn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2vxqpekqu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hdocugat.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2iofjkokh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vuttjyww.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tosgslzw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kzolzvmo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ryabmhsk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2tnldiaen.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xmuydxpz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2bsejwscn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2clboowsr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gevcfssj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ydrudulo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2mjrnhaet.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ofdltxdo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kuzukibc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pvotcmax.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mhovpphq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ktsmvvrb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ujbojflc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2lytxnaxi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wravrvfo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hhzbaeps.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ujlghcvw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2lahazrkx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jspfphbs.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2xdoildge.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2tmrydfpt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xqvfcovq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oxcapqtq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bmkbuslc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kmmrjbxa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2bgbleasg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2raxcewtn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ujtflzil.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2tebmzfvp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2mfkfujpk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ezoldkni.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hapcjyso.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lyrehdmk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2okudeacb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2snranndl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fmkmnrld.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2xfpjqfpe.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2hklgepaa.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2lfsyxteo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2cggfkbhl.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2qsinkmmb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2zppgczry.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2xozlbtyv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ikvqjhuv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ycizlxhd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2oyhjmrzn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eggskyvp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2yqahfyss.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gsqggrjw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2jytaphax.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2imvccmxw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wnqbdkge.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2tsyqhvwe.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wpgdhhdx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2fsztffsy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ctwbshez.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jjxyezrp.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wutbttig.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wrpispce.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bsofncfe.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2pacamuxu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2youaalxl.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2yfjzwubp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2qdyjdixj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2qqtpnwbm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2uhzekzfy.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2sefjtjlw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2swlpjesf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jsbesqzk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hnwxrgys.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2spzfivac.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iygzntrx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xrgistgo.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zjjjedsb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2frtekxin.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ifaidmkj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2gaqrtuyv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vheijrcp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ifufvbqi.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2merxuhgq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ptuytckw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2nurnaubw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2lawnnszt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2wgzqbxeu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2icspsaca.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2srcztvtv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ikzmdwll.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rgeppohf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2njuqslcq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kgiuwbjt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wvxdvpxj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2faojrdqy.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2xtoxqqoe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2nabmbbjm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2zloukqmt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2vbyvjwzi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tylhgzlk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xbjtcidp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2tyshqxtt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bqoeneif.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2zxjfoirw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2itclxeba.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2lqkwapnh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zunfinwx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2lpjalntu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2abeilkxk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ndrnkrpv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2mifjnrek.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjjxdatf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2nmsitmwz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2lkuahmzx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2dlvzomis.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2uadiafwp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bujmbphg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2strxwhsa.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jywcjslf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kficbrup.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zqxgwrkg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mwupazfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qvlrwwdz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2atsmwlqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqvbrzfe.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uyugycqp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2qpwrgble.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xlqymekr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2surdhutb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qksoeker.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2whwuvtry.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2glxcrcun.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2gaaxddqa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bubxmtmx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wogqordw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dswxqsfl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2qfahbjex.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jlhhtpqr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bdnfcnnf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qvzlvqmw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ifqxguvh.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2uiopehfx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jceaxqys.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ayrhcozz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2cnvrbapf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fculzdty.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2olqwdyex.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vkbxphbt.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jakiszlz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hxbrzusk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2hkuuygxq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lsqcfacj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2dtfwvkkh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2neluezfq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2yfowpvoi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2lofcnyhu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2chznguje.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pkjjixdn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2gxkebvpc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ykzyxjeu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nyjinjmt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2skewjrga.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2tdstwgna.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2yhfrukuw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2odprupim.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2kwforqxz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nzljhmxk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2kzgfpfwp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ellvkuit.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zuylhbak.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jxyzxcdq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vtrufosz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2sfacwzzw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hsdlcjog.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hzcbnwes.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hqzhamin.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fmwruecd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wjlkqxpm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dokjpscx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nxbjztip.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2taiikois.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vfafowji.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2nxkhpkgi.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2tclnsijb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2kdqejhxp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qikkqcgq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2yisynaap.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2optmjcye.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2mvapxxhz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2kitblpue.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2orxfzssz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zvhxrfoc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lhnyhhfq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vrdnrljq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2nhgneeom.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kdhrjoft.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rzhomwzw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2hirgguem.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2gdtctebb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2mjlskmbe.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2scblbkmf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2dqudzyyv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2pqwiazsm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ziojhiwg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2plbdmzpa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2aweftqoc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2xtnzhagp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pnscphbj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2hwpvbtcl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2siehtall.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wckponnc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sfoukplv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jzdaemob.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cigyagyg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2mggdabbm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2cdtrbgdc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qlitotay.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bnbjomoi.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zhaicgtf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2upzqzpip.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cnkqwanx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gjrojgkg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hdxjsxpe.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xhrdyewz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gxbyyheg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ngzgzcnt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2acufqsmt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bararkuh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jijyyfrp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2gdinouno.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2mxcjfvkd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fhulpqfk.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2qelnrsog.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2lproishz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2janvhchr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtmmpmpn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2llsnoijv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xowuygyy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uztzdpfo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2sowrokmz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2tsgnlcsv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qmtfkuka.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2bbekiziz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2owcuaakb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yqoekhbe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2hhcwpdzw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kwstsami.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2esszxqis.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2kcrtkbyf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2crmlzfvj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2aurfcgip.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2uhxbquvb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2inzdvfnd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2allhnvmy.html


<!-- 参考信息 -->