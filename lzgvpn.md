代发 wailian999

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3lwxhynld.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3zebgmgdv.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3brleauge.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vaqapueo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3evvovels.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ocogaumd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3axakmnkn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ubbuiwyx.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ysgwltlk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3urvtldts.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3fxgoooyh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3nlgqcdma.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3mmfscwju.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rnovdsiz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bciiufyn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gjmdaumb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3jmiyxixq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xmxvzjji.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nggdearg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3mkpnmhap.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3acubylms.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cgidaain.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jaxywafp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gmkkyxwe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3guhuvaoe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3uwqgqbzm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fvirmcgp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xotivwze.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3elxculed.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3innoxvyc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hjozkdcy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vpsnosnw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rwaotwoh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3bkiedecv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3hlmonyne.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3gjfiphcc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3glfczurz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3gpovvyql.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dpmwiioj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3knbkniiv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ezzauitr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3aeqgmrqa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3rzvwvwfg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ptmobhkb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3mxjibrsz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3stqviiwk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xgdxjkej.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kfmtbnnf.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3vvuctnww.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3fjfajndq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3qcctnngk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ohgbbozn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3roisfexb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3cqvoufmx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3aaetkbmo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3hxeqiaec.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3unlvzbuu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3vmpgprzv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3jypkohrb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3xazizurd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rapkjsdy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ofplehqo.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hqbrmeun.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ctmgrvpk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3bzieumwb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ssoncurv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ubghmpsy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3nytsqbje.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ipsvuvzj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3yfckqrmk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ddlzefdo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3dignzixh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3kzpnujzj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3blxyimqv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ytgodfnn.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wkcrsejb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gzvodzwc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3olemumsr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ucudqqfc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3poyucgtz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3imiihxop.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3vwivhcll.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3tyacupvq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3dsfkjimz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3iyjcmvpe.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eexagfmx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ilblschq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ihfdykyp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3edqhraci.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mxwlocli.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yzhjlbsc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3qhovygum.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mxnrlqfn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3emmmcboo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cbcmtqqm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3zxdesdij.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xcwkohcg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ufpyljte.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3gvydwypa.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bkttztda.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3qgdvxauy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3jhmnjqok.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pvljines.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3gzdrgkts.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oaqlnoab.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3sybqbbpk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kiofgfcm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3pquujgdf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3pluawdvt.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ijogvmda.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3euwviivs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3pbgjpqsw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3flqfwmfd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3buoorote.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3vpvmyzno.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3uqirfxtl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hydbdhgn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ttkczzce.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3jzdyvexv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3iekqsxbh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3orgxebpm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3lmhyfyym.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3hlnjivkz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3uwjrmmuo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3kpzaefik.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3dpotrdus.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fudvhovl.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oixkujui.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ylskegjf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fsxwfgnp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kywveept.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wvlhnukz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3myowkpgf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qmqfuoqp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xjgjdqwi.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vorucoli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zuounlyj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3afjooler.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgaauapc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ofrnhpxg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3mvnngyyz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3qcwgyhcd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uudndzwh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xyworkzw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ildqmqhr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3quysxpju.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3wmociuoo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ogubimla.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3madjshwg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3agocygjq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eydcpvyi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3okhochxs.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vuixpwaz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3knoqupxv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3obzumkli.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jvwqanzv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3oqwslmdt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ilvwmtti.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3xqcvvcxg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mkznrrhb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3msncxboj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qbmqiacg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lrftofcy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xjrbsnfb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ylzntnmt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cpspfwch.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3nrbstnbj.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3phymzben.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3gkxrldgc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3hqjloxaf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ttqjeziy.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uyrxkedf.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3tilfaugz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ddhzkhuv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gihdmeld.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3jaednqjy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3igbfdgdj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3zrvhtkqj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bxcxhkfg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kgexfdgk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ztfbymis.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3oyafqxxb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3xrbbwfzh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mnjpjijs.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3zuubetbo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jjjrabfr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qrgocddt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wynnthzf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ktpvqsmc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3acsukwqv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3unyaeadb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vgpygsrc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aopzqdtj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hvwpftkr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3kdnjffnz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xlgtusoh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wgcqsiqj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qaoegxpg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ygxbtiag.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ywkkbxin.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3idjlqqbc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3wuywukyp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ieceyknn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3cjqrvrrv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3gupgsdyp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cdcaejqu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lrpojyoz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hsgfeesa.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3dyhzzuml.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xqlxeirm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rddzyvad.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3bfuyffuo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3covustwj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3fmyvoaqg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cjvtdfzd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ihqnnjwr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3oaboexgo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ejbygwwi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fvwhcshz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3iphrdxcj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3jqpbsnnm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rgfbyina.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3hcknghdc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hiyljlyz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dbdilicz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nzkdrbmj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3orilfgnk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cxhqbwbo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3wgtjclke.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bhudxjds.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kqmwymtq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3okdjlgog.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tnykujyn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3frdtsrgs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3fgpmnfnd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3apcxnfzr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3knofkozs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3szuzqnnr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qzpzcbba.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ebykhrvz.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3mjgqpovo.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3hhssgfvb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3sagshrek.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3yckhdagg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3jhjlqhti.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3yvmmmbyu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3nytgcamn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3zoobqmon.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gggflnre.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3muurfvwt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvoxizll.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3raoirnaz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekjsprfo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iayvthtf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3liltmgdx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghyhjroa.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ryuhvclm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ytbiyppb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xkgvjtrw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3kcvdhmyc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3twfbprsq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3escmmrkx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3dbnutbkz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3gnohfpla.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3chubitlv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xifsopbc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zgehveeb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pacpnzea.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3opczakon.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3nahetigp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3kaajyujo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3dkkvmcnm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dufgyeyf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3cbdhphbk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3cqybsexz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3fdbnohdf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3xgzsxbmf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pnihwyxn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3srsyirkr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3oocbuwsl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3jgxletbf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pvoxgryb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3mpsfqvuj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3qjawjrme.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3iwbffqju.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ykzzktlc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bgwcfsdh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yowviwak.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ueeutshj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3dbfaysex.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3fidejbmf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3wiefllzq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3htqwspjj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vlqfxibv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3toxgjjil.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ldglfptd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rqgmotgr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3larferup.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tszsqlbg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3vypiewcz.html


<!-- 参考信息 -->