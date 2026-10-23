代发 wailian999

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kjtxoegi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3gvsdnofu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3jeodnlgm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3eplzdccl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vtkcadfo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hrpycbsa.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ahrwfraq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3aqghrhjl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3azlejhlr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jcsfequy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pxelpetb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3itdfrhfv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3njijxjti.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3bbjswxdb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3cothfedk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3tepmptwo.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3cwgzsiuf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3keilnpyy.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vslpkmdo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3hbjuqtsp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bumuglnk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ugsuabtc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3crxyqcie.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lyunvsby.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3wxckwdtb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3asulfqqy.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3phshbcds.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zefosvjg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qqzgdsif.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kkgfirqc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3wmzzlgtk.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rrfhbsjd.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3npzafucc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3vxyvdwkr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3nicfwuwx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3dvwsstyi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3otthqtvs.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bcfkloah.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xnjjxycn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jvnwcysb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3mnnbwqfl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3fzlsfaui.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xfblbxkg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3cppvydjx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3uhugouhc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3smpvpdhj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3goaojdpt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3umrxfzhr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3wbgdakss.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3aeejajnt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pyzxxlqm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nfneldwr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3icwimafp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3erzknxbm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3fjwkpfds.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mmxhuqpy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hkgptkln.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3jruiynuo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3bgsinjfr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3rdkecnub.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3jelfmeud.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3gdghzerp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xcxvhirm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fcnrnqjp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jrwfeweg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fkefuxvu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3hdfndmoo.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3tracppea.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3hzzmgjfc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3zzsgpwvz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3zpnusxjv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3krdqtafb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jxabxwzr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ahnoscfq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3wgskmcnn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3icfpafyc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3scfkxhow.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ieoohpys.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3aopxvfqj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3qukggcml.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3rlmbfujt.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3zdkuwmeh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3imsageoc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3xjfqwsow.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fxcqiyqe.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3sugtfcre.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3jzfcjfnn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hcuesgzl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ldlojmpc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uiicguwc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3mlvpyygw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3zrziekts.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hfftlghl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3soevwgkg.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3opwzqtfp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ahkkxsih.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jkcngpqr.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3jrjvaxoc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cwknwmvr.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fixdcbav.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zobwcisi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ljgpfzvv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ysgecmip.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3aibddjry.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3lktxuqif.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3zlphpuvr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3kgjzvjli.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3stmtzttk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vbbscmdc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sjrxurch.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hkplyeqm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qwgtdidv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gnuviplh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gzjzqcqz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lkjxmedu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3zpkwjcta.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3liidmcby.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3mftdfpmg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pgazoews.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3krarulko.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ashvifef.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3yjndbgdc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3qnsdfezo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yhyjqrnf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3chtclpqf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3xjkvarlr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3spjgamjy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3osmzsujm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3edoituvd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3lqghgsja.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3echhpapn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3dfckqzva.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3fgrkvxah.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3rpsimueo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3tvctlzdi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ojvzqlks.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3viwgwblq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dmphbpnq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3cmmobsul.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3kazyvuyr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3nbxiygjv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3fofomplg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3esvzguht.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3qciifugl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3bekjlndu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3jbtzfswq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3nsfbkmod.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wqjeijtc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3etludjah.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vtffjpqh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mdgduulc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ebcihzrn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3emzxjhja.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ptlylxvj.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3whocfneb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3abpygvsp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jhvdavqr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3hfujwdli.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lflkbdlq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fznhbnii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwmyllxu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3opsoafxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ykbogzlm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3twdebybm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3wrdumqzh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vnuyirel.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3uwrbyisf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3mbflhznb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3kqeginlm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3etqaxifj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3mzijbnvp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kvnvuzzj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gweinlbk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fdwybhnk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3zklnlevd.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zwqpigpy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gfbcfrwv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bhpxfqyw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3frywwofe.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wtdhzmwm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3engrtsiz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bznblete.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3riglgkih.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3eauynazp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rnfyqywk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3sgpzdvpe.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oerxarob.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hbaripem.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3imblfavq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3bembizcl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3kjwbdhdz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3uffbuvsx.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3btmibynh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3dxhnufsn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kwotjbul.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3eikzrrby.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3bntfuejh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jxvzqeoj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hlpgsjuh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3qollcnnr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3lddwedvt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3yvkpaheu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wnydcgeg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zrmwvbsi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ilovgalc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3uuwbdorc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ppvpwtpv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vblppenn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3jtfmvsnb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3oleljovb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hwjotoib.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xdkvhohs.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ihyzqeqt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bfbenojz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uvxprghf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kvmolhus.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sgkdcjqr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ergghwxr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3bttadyub.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ggnmfqoz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3mfrpfklo.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yupnuwkb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3hujtyrfj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3bchnxrlm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3aumgrjhq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3zzdpzjlu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3psgprxfl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3viadviot.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3vlcdhyzt.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yjqyqxcl.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mzcirjhb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hqnmochk.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3qftrlsps.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3imeyqppy.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3sdbatcmq.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3wkffextl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tftcvvlc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3mmtoihmf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gagnxkql.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ljxdiuap.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3uknapzvu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3cnvsgobf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3clawlesu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ejmrxzna.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3exokqvev.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wyrgvmnq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3uinslelx.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3eibfxjen.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jmjjqems.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tqrpobzt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vqfzqtvr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bmldjfhf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3nkwdlvmt.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3whdjvilv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pmlcurfw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zasiecjg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jyvhzecm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nylyyfvs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sdlqaxvz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3stphjqpc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3sncyermk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3tzgnhxnr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fatrrrfk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tvxpcvcc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3adqvvbih.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pyukikmv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3shrlcgqz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ihmduomj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3xujbiafp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nwwqmovl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3qkrzjglc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qfublqtl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3jgssxnry.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnsxytbz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfllqipx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bhefqvzc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3szmrxyrv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rbsotvat.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3tjcxowpn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqzhzjvl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3wmgxawnz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3vmblofge.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3scyorjwo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3wmsunhwa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3avheylhc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nlxlakyf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3lcsjaxxd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3toydrlmz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3oghjuzzq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3yntlogaa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3narwarlm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xrtgwary.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3edsrzhsl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ucvfceze.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3krzwzbqb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3otqnukmr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3sswpvwpo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3orcvvlbu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bwphevpb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3abdglroz.html


<!-- 参考信息 -->