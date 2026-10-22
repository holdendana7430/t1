代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2vhcvrxwc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2szqszdlc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2clboijim.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ygldlqzp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kkivptdu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ohcaabnk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2nclyflcm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ryldenvg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pjtqfgsh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2lchklklh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2lnukdrwm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2vrztkiir.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qbusegta.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vrnpvdwe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qmlmoqnu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2unxiopxp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2rntqtomb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2wbzmdovp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2akbryzyo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xrzihdun.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2alxytrie.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2jqaogubq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dxvfbzhe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2nvwulfah.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2agqhzfeb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2azietpwq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lhdbzitb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2nopzfqgm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ldyomjsl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2rnkbpbey.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2slpzjuwg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2srwbtsuz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cgtrzuzn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gynhkpzg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2pjuesbqy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yxxhulqw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ghdbpgqd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2sidyvdks.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2bjaqrxdw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rscneihb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gszeesjs.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bvcggera.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dzvmbksp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tooyuzzg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2jfcohubg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2sicshxfz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qdqnzvzx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2zsevosja.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2srzjcjqd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2naunahbx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bnmiwcuv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jucmyldt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wokqznbp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vjznprhu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xqzmofrx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yfheoyfm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wjomtdap.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2czbmxdnt.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fcasktbt.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wuyslyms.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2drjyqiun.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2egjhqtbd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qngrnbni.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2rytudbwh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2vxsgceoi.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2avfesuav.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cantnjyz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zeoanrst.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fjkajdof.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dyupsruc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2auzfoipx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2uokrhqcx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2eqnxlesz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2gnypjmlh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rzjloasm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2copafdly.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xjxzmjsj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iycmihek.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ebouwirj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2cighddbg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2palemdvq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2mitcqnag.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2mobnalov.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2myecuhpb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2eywhswng.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2jfuolcdu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2glzultyd.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2msimmpcw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2crgxldse.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rzgvahvp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2wzsyhslb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ubebifeh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ejnnuvuj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vzngvyda.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2dqaihedk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2mndxwwqk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2epdwgrsq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2vdrgebys.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2zwybexzg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2jwyocfhl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2odztmisf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2pkdmgfsl.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2bxmfoopr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ewldhqoi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2sleybkms.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2pislukzv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2wduphddf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2lcupetqy.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2mpwrugvs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2esgvnahp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ejvtuoay.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ldkttdit.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ecxembvx.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xuyicapw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wxvgubgn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tqyhfaef.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hassttyq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zyjdeyzs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2riuasmln.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2mwrpqhiy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2blqruaod.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2wqrlksbo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2rgwydhvr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2tpyquymg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cvpidfcb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vusonvgt.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2hbtilxdb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2dmdkrsbj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2pjonfyyu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2rcbxwhzb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ewfqhxzn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2murfruva.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eioypbqd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2oponrmpr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2byqvxofj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ykiudnmg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2jhwjtffm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2iqaqamap.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ysmcdcrw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vxujcdqt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2fndckcjs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kmbexjay.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dodztasa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qdggpawc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dvnkpoel.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ipcmvfkc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2eslhbukg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2sbyapjqc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2snyrnntu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ejroilte.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2qkinrbbk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mfaduurh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2xseuhnav.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fexbrcqc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2piqwavkn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zihxrlnw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qfwjkklc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ubynzgcv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ckutjkwb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qyjgyhoa.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hbkbuzqj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ntzuodxh.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lkwyfmqq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gixibtte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2simfbakg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2yjauugey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nlvjwsnf.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aifjebql.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2bnsttoeb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2eyvqfcex.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xexbjvku.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rakwergv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2viegqjid.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ekvpgclc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2czcpdfic.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2isxmtwel.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2qvvmtkws.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fhksvnpc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vcjhzeai.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2msuhohxv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2senfdivt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bscdrtxu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mrqjyuuy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ydalzbgl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2oauavtkb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2irgnfvdf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2trjdipkq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xhvnrvds.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dnzcjsiu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tnbjitvu.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bxjssdrz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2omnzoewx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jvrliyvz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xllezqwz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2kzdyokia.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vckltbtz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2eatlavee.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2txtfizey.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fnxribeu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hswggjwc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2gkhsbygk.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2brzpymvm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bnvpnlhg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2cvgqnyvv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2wexvedfv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2txuvrmhw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ocxodhuv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fkwfeezm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rjuxefbv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2pxmktbde.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2bskupqzp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rrgccmaf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2dkivsnxb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2twgmsrqs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gscbvoqw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wunxyyqp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xfxpsjdy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jlsahdgh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lpkovict.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uahbrgff.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xhjaxexs.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2stpgewup.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2uxippmit.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fmsxpcfn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ybzacapy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2zqgguuze.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2erisonnu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2bbirpflg.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2bstnemac.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2buytxvzh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ihxmwuay.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2hiwalrjg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2vslbivkz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jkttxizx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2otwtpaxa.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rglcouzp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2qdrtysmz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gskbwlzp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wyxjasbl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2lfclbrsp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lewbksji.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2nscncagp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vbhgzbsn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lavekmma.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2argegilg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2pupxfavk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2izuljkzf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bfoinbog.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2dlavknay.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cibckyyr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2bilkpyed.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lwmbyeqp.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xfqlbvgf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fbuhqfco.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rqhqezzq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lxjpluwy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2snttilty.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ikrgnyae.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rghaoysz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2icazgypz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xygjcbmz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xdftdzbq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2qieawulk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kjgvqhvf.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iogyfudw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bwnhtrqv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2vvvedsbj.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2htwnmsce.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2euffblpd.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tymsnakj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2eeahmwdk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2plwzbcbx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2sepzksic.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2niwhnlny.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2imqxhyzr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2jhvstbxh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2gkhcxrwj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubwuotzg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xbivwpkf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qekfeirk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjgfmmda.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tkoxkjeh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2dnbjtwza.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gwrfdxgy.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2uvitbzom.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2uvzoamcz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ooikakad.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tgbzxqbh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lxadnaez.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zsqcswfs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2lozsuzhg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2npfeqsna.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mzmvknmj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2kieliadm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2fzvuqhyw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2yvilfril.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xkzjnuls.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2oeyglvkw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2xewuzvqh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vxnjlryx.html


<!-- 参考信息 -->