代发 wailian999

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oqptwrcm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2csdpcvtq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2tkdpmsck.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2nvrohtbt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2onwuxurg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rvmnwbmc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2fthzacvk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2saxlekbc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2inzkgbhq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2geuwaghm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xfahmltc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rkhopybr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2rvlvceob.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xiiihmgw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2oqqqekln.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2geybchge.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2yvwjkeeb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2qklicoqo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2lqfeaesl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2yvqiljlh.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2cspdhfxg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2krzmgjzv.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xkasbkou.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2dsyzogoo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zrpkuipy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2cqrecntt.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ofwpihfa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ktkqzuwp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zacfdvwh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qythshdk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ojcijajo.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dqsbyzpj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2wsanklqu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2cnyriwch.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2hhocljdu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jjulgkrp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2vctfnlzw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wuahiewe.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hriaxugw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2wnqafjvq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2lnrscgjx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2jonqvbkn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ipdclrbl.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2vhpsyqbm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2qiuoeyuq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cpalzubq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vvclztkq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xxrruxaf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sgamcjog.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wdmoguqg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2eopfqlne.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nabuzryk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2dgxzyopy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xbmijnsj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xczyqnpc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gcpnffwr.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bsthirky.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2bidjbqqn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2apeglgiv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ngkkmsij.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wyhvtyhg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2cmeraifa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2holhhlki.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yfkhoyeg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dysoylru.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2yauyqfas.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2mahnudyb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hesnqhjd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qvgyvegy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2veijwlpa.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ytrsmfgs.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2myceipyk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mhcwdnce.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2urihdmoe.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2jcdwncnf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2nmnsjquy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2uttyduzh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2vgazxeqc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2gqoswyzj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2vmuadxov.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2otrsuxwj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2zdfwajgl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2qasukleh.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2dkokahfd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2jhkoufnv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2mratpvbh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2jzpncdnn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mfbevxcf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2wcjttaqb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xcarafcy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2swzcrbkx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2xsggtabm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2cbteirsd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2xmsbdijd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2bjbbqcqm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2oagqqyoa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2asiaynlu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ghgfvyux.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2kzkpornx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2weeydenq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2cobmkzgi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nuhhlyqk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ssdjhygz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2jolrdcbb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2nmukuayc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2qwceirif.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2mqvhaobs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mubdfblt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2qimsyasd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cdhcvkdv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pvexdugs.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kroimhag.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qewbdusd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2udydvokg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hybybzif.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2vjfpjocc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2avjtdvgd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2eekyhmig.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aernniln.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2tqykbjtp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2erxsieps.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2xvcpbeob.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2kvgckmqg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2rplkzvlk.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2erknxazx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2uvwauelo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2qytpetbh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2psdqopjw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yapzowgo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2yjquqkgf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gbkcygoj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2seydmrux.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2svvyyawa.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2yqlwmmic.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2vjtgoeho.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tduotwjd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kycgnfxi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bfatmpwq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2verwvtaw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2mtclhvsf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2wxxtmraz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2qbavyijx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2wgokhowx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ssdzninp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2tgkupqqg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mvljuwfo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2gfyvcwtl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kajodldb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2irezgbis.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2keyhcaak.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pgvudmbd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ztbjtnkh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fqaezaxz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pqogrcgs.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vxzmjvld.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2soeuwyiw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2uptihnmq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mzftxxmy.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bqgnteub.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2idddokyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxrthgee.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2wdnvdcek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2myqnyrys.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dtsrmgzp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2xxdzyoxf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2jkpfxqqu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kbeymhxt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oeyrrigv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2klickgzx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2pdgpyfrt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2rlvugtaz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vsoufiyi.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gijbqjhu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2slijdisc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uyjbvmbe.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2japdgvyh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wwgsdxus.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kuwpfwod.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2mugqkidq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mpdpxyxs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2jmnbdnit.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hidqgpzg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2lnvnzmma.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qncpvgcg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nscwmjzh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2auradzkd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yyoqojah.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rmquirjj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2sygcsnlz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2aeaarixl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2epgqvkpp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hkfgwzdc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2qngfdtdk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2qqsoqzhx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kpwwzmqz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xltbyibo.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2butkpkcc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2yepffrpp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cabvykvw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bdvcccfi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2faqkbaok.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2idtguqea.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2goowquue.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oncjfvqx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uuscyomn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2sfdudeuz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2wfnhcuhl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sbavksqe.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2mrxnoceo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ohgllypi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pxhfwply.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wupzymna.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xcjtminu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bctwmidq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2tdljrbom.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hpjtkqxk.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tkdgynmj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2pufrpcso.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2kpdorfjh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xiugusnt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2qxkczdny.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ncozrtjn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2versdlrf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ojanlylb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2lliqqmwh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2capxtamp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2aargabjm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ryvqlqiq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2pghuuacs.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hprwurre.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hjljmios.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mlefygvv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2akhldlpi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2awklysap.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2uxdfrlxe.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2lctwrsbi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2jmtuazfd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2hfsapabz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gesxpwzd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wciccnto.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2yhozlppe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2rdodfgdz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2nbuqhnaj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qfjapjgo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2qfjdcmtl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nxsxtnne.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gybyopkt.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2aqkmshpc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rprouddx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gsxoqfva.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pjulsleh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lxqshmrd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ktindtdv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2njndikwv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vbrvcfkd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iblesdjw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oddiujux.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fjuuactd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2wdmqzaib.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2iwuxjgvm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2miggkscy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2crhkhrbn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2fcjeksdg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ibussend.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2asaevrfn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rcmvsmiu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ehfuwyxr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2etvypzwf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2smnxpyvk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vssyywqy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ekzzuwlh.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2iunxqsvm.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2fkbfpgbs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2dyjobiuy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hyamsfte.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cevjuzgp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zdkrechw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mbujkney.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ejgbbubw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sqowqoyf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2aesxdfrh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2rdvjyqsx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2jnyakoxn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2twxnfoma.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2yqisdumh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2eywzvyei.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2xubvzlay.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2euagdzuc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cymjjtxw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2auqsytqb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hbfgrenj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nekvypst.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2hbuwhqen.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2pzfkmtbg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2utxznivy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qucyfswn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2phxolfki.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2szgihwnd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qistgmvj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bffiejjy.html


<!-- 参考信息 -->