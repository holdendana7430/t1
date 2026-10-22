代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2dsrskfjy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2msgfmcmx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2enmandhd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ovkxajmu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wweuymha.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lbubtyfs.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2cqiblpsc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ydyexnjs.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wkguxbfq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ljfppuwi.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aikjjkik.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vsmndbmc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2cluqlbyb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2zvzafwpg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2misdzumh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2xdrmgkee.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zxtlhnch.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2irrnzuaz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zdtffaeg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ynjippnr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ljwxumry.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2hxftvzqv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2zygvghbp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2laniypre.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uugtfvyv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yljopjwc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2hyinrkfb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2xuvyyddw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2wyrborey.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nxvbxcvp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ihczoxag.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jqvijzbp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qubumckh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ivvcuxic.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ypasbinv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2bogpggry.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2yjscktrv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2cdwqzzsm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2jbmiefba.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2kesnvhnm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hjwkzakv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gwcgyvgr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wrhupmbt.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uleiaswo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2idqqojed.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2pupenqyj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xjumgwuq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2auhvmejs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bomlhpof.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dctovnqy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2wyefgyjr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gpzyfbxj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2kgttpnoy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2jtyslqey.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2slkuohlb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2zwieshak.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qakyudbj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fygqzsnj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xvfmwkoy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2nnzfqpuk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ppwxplpx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2btjphqnm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nlibojtx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ojhuwjyx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ieoqlchu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gcfsadjk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xlrooxim.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ztubhkcs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eranfeix.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rahbrgxj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2afyosamx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bacsoxqp.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2efvijmgt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zjgmrxit.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ftpsdwrk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2akybaaau.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2weqxvksf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2thlqdldl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ewrclsps.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2zymwsmfa.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wafgacqb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2gevbxaju.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xxvhstro.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xgbrzntw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jahinizm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hjejdnhq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2wrwmcsel.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2gjjisxls.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2nhxkvfgq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2cwaigrcu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vakadjhv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sntjdcxu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2keudngxp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jhvyxtpl.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2warvcbrl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wmpjiafm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jotrgpca.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ucyjsobz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2fzslfjik.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2btsdqvqw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2egcxcyvj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2yidtzady.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2pzrewutu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2mbhibfyp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2yopbjull.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2pkqyrihc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2gwjnfjts.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yfptpfjs.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2urivnuyc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ngstwcpb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2kuhrcaym.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2hdckgeok.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2fjklwkch.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2xeaqnsfb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2idvsgcup.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2aviivunp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2vipyugtn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2qgwwvbhg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ywskpfsz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tukzgeil.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xholagpp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qjkykdvf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2degnirag.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2lmeqxhme.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2rjvzcayx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2bqinbqwb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2gfdegiip.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2velmctrn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jjuhbgps.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tywnzapz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mgdiqrfq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xhvemwqa.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jfccwtqn.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hljedzlb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pcwyoixk.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2rdmhqoac.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2evatszfj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2cvozgesr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2plnkdmas.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2qgdirspd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zyozbwsj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2tvdovpmy.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ddqfyzdz.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2yrbnyqqc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xlssvopn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nrhzsqnp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fdwfztwt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nimikook.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2difqueod.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xgtqjyzn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dmeirkuh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2iqdxonsz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2tudibsjr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2uaiukdzn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2uhirgzxd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2dfsoshke.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2luuoqpdq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nnjuamke.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2cxqisszo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2aqklqpsu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qlgubblj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2narikggx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vyiatykc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2kkaubsxq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2bbfcwlsz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xefpxxkd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2xeudiwqw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nmkbxnvp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2jxktdykv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eczucmpz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uajolkbl.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2kpfxvbju.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nsnscudo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ybmkvghy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mywdkybb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2umdxfhnt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2yczycqvt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xdbgsvir.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xujxdpke.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jyqjpwyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2knyxvotb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2tphyylib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhaeithb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cjxtxkoh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2zjfohpoi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2dczzwhko.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zvzctltz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ikczbacb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2xgyusnfi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zrhwrphd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2yljhltyt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zbxujtkj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xsbadsgf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qtrtqyyt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2yokaomvh.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wsifdglt.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bcdxmnnf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ulxsarcu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2gvlhhwlk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rsmnsutr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2eyrgzvch.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xdjvftsy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2mhgectzp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xsndymfp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wbwukhjy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bdrqfhvn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2layfplym.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nkrhwvov.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2nninuhhy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pmctccis.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2idelzmsv.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ruemmisa.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2imsbnlny.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2vrnynama.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kzpljjub.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yrzujabl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2exspeajv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jpsdysrr.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dehwyzie.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2kadisegb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2gmaieeto.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2dpdjjkdh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2whhcxuko.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rpzsfume.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rpbczqbb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2vnhbnedc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2balmbwdx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qtmnukoc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2klqyxqvd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qvwbojke.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2gsgxaouy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yoelzlkf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kddwuehd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zgthtgux.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uijrrnvv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tmsvflci.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2obyijsmd.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2diejeyxh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2izvyewsp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mtnxofdx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2hordkyhy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2fbbideva.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2tpbpnckj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qmuwndqu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2awaswmih.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2sppchnto.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ckggvytl.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2avbvwqyh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2kcovrihg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gksjwgwk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2etyarnok.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2plgnkyax.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2kitvrpcm.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2trrwmxra.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2tceuvoyh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2llnaxbbh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gtguqkib.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2zgnfekmq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yzicrace.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dtycaiol.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2uzeuigeq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2akfgazcc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2eltkaimh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rwtqsunm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2emwkwgss.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xfdgulme.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2mamokfff.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xyzarpvy.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rlbkdncn.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mvpxgwsb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bmakvqlv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2slttkxee.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2bhkibwkv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2dcberouj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hlztmukw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bfspobhf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2inbkevxt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2odewbbqp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2svmtrxoy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hqtdaiqe.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zlypobdp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vigqueoz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hbxvwdsx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ewjepeyd.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2bisaqkyf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2otbbefzz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cdncrpmy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2xcbxxluo.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2yaxfavsm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2nnoilqtp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2gnmstxuo.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zeepebpd.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2kqizoomv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2dlhzczxe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pcyzacfl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rtyhguzq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnwubiej.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2uvshkjbw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2jlmyehak.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqihgrvd.html


<!-- 参考信息 -->