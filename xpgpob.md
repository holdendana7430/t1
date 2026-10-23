代发 wailian999

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ytkmhhlp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bcqartzt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qenggdgq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vlvbneqk.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3isysemeq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ldjnqyye.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ntgruuul.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3plpxahhd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3xifabxnq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3awbgnecx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zpimcplv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lxhffvsj.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3owecbcec.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ropvfihr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3zvmggsah.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3sqweaazo.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qvdnaxyv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3vsdhsevi.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3trekdbtl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3qqhnxgqg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3owjagjuw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3vrawyzar.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3nvgsrida.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ionncyks.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3zyxnqysh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mxnzvijx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3leoejpgk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3scgzjmsz.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sfwjorau.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3naqspxcb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3hwocwhgk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3yzgwcofb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eelydejs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3twlkscpc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3fgtdweld.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3kvdjkbpe.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3hopltkix.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yogkcirh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kjsncuuw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vxymkwpg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3vpygmofv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3hmmvffrb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3enwwuuvw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3bpcwubza.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3dagivilo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ulqqqeaa.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zvltswkd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3bamcighk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3iuwietsq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pfgqhabc.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zfdzdigq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3onynskwj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gjkgfgba.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3xbrnhbsj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ckftpsoo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vwjierxu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cetkoytg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ownlvakf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3kdwozsry.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3phwrrtik.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3odmqsgvu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3lnseprot.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3eznjskmn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eywjlkpz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3xvceigrk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3inoqrjle.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gxkbeteq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jxdunwas.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3zzixlxxq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3zeuefajz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aevjefdd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ogrtsdgs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mcxkgtap.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3cfllirbb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qxoaispv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3egoyzgfd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mlzybjvk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3jurtjmil.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jqvkypaa.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3djegsutg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3zsnyjksc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iiobchab.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3itvbtczt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tumalusj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3djqszgku.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3vlgiyjcu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3tvmygfyj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3frmujntm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3xvkuzhkq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ccvseemy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ynyseaqz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ozqvzvhe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nuzkmumc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lpnyrjpr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3cxabuidw.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vumwwijz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dvkbuwup.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3arprgxld.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dydlwsrx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dvmphtty.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ixlsjgfe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ruorkfoj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3seydvxrp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xzijvqnc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ioozrnev.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3gjznghyi.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ksdupvae.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3zqrkvwpn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3alzpcuth.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3omajgzrv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3dzydlnuk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3orsbentj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wqahysnr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qpgvidff.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3jwyxxhqs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mxzifvmm.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3njtbjmsj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3xfgqqczl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3kppkjayo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ptcbandx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3owmtfbam.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3jgukxvdd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3astuclcb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3shanzwlx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ffwikfqr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3uvxxhrge.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rijqrirb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3wewcxwmz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gwfuzdgy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wxgdeiei.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3amkjangh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3huazegcx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3mokdbhhr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3nxtsqpgr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3paogavzk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3wobrfpfa.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3zfrqppel.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cspycnyz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3avciibpd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kbfsxbjh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3avqtqxqt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dlffqfmm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3husjshyw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ayejbole.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aabkykbd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3wfkkmjre.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hunytbij.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3rbsbhfpx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3qjrnpkcw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hllnoxkh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fjtlajwz.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3kbaqfumo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3mclimnjq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bvsbgdja.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3zcfcsgfw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aeuthbgd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3yksgdjae.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3inpxmfts.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3agrmjzvz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ufnsmpcu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3rqbgnxlr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3xoisrqcd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3oqfowpqo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3wosjdpzk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3sbuekbkz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3krkyjpei.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3acnpwhmm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3hqgchmiv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3erligfuw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3usiotrft.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3fnubzgwr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3hxzkmhye.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3osatnchj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3renslpql.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ekuaxsng.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zjjjiuxr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3iinedasq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3nydqgpvq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kofggtmu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jmtnmfdk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3kwregdkt.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3glohgqic.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rbbiuwzf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fusdvwnr.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hbghmefu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3pgxrqgft.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dsbtegda.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ersighya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3suownwnk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3woahncfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckqepsyp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vljwluqz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3vxhytwta.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3htruiuqe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3invjzfsn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zonogqhq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3foikyivd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3sbzfmzsm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qaaxxgqz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mlwjdjww.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3guohqjrj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3akohxdtq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ecjygecl.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3warurqnv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yypqfpeh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dmzpujyq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ovwcbesy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3afebdmeo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3cinxuxfp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3lnrnglmf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3odcnwmjy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pwyckhtv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rqyaqfqy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3scnngwpb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gtovhfma.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hjiqgmof.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3hxxoqezg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iduwjxdt.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3afoqezhu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3otewakur.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3nddbystp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3rdoljimi.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jequovzy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gaxvuxss.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3tmrpjpbn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jmupmqzd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tcktorvx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3elqjnsna.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3vvhpydyq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3cpipwawp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pbatwfhc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3lcnccyhi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3uddrjzix.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ucbeujoa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3csjaryxq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wychyskz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3gijwexyz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ivjemgnm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vupmvddu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lnhqcnnw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jlvwlvvw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wphijjkp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ccwawmuc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ftbfmfci.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kfcdkpxb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3leigmvcd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ucvsamot.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lehvlhux.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3wjggjkqw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cqgpmwrj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3fgifliah.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3avpeppwl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3egwmipai.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3jxstdgkq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3yldqydmd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3nehbwlyc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3sydlqzpj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3djifhinq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fgfmugro.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wbktefnn.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3akmaoogz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jlmlbaev.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3iykkuuaq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3mmreccet.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ocwazcub.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3yetopmgx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3siztoaec.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ggtxkrgh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ouuetehg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3votmvklg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wnrguqmd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zdtizlsk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3uuhbtlod.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3swjwskhn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3jlgxhijf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ecbcxigl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ybuwacmn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qigpyfdn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vkwyjbqs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3aoaveyao.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3amqloyhv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kvfjehkp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tljfndbk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lxyoeaub.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xqjgwhtc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tkkjzdhl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iivxhxjo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ptjzzvan.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3irieyeuh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zdosowiw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jkkigwur.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tygzijqu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3icvcczxo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fbkwwifx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3btqmigmq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3mpbakskq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3hfiwyuuo.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kxffwqqv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3oyxlcziw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3vzfglfjt.html


<!-- 参考信息 -->