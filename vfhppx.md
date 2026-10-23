代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fozfefzi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vlvaagmb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3nbhymcfr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sqqjusbm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rwjbvrfy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ghfjecvb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3qmxvfoik.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3xaqcdirc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3magsfuyi.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3nrtwshzb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fbxhpmpd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bmfvzsem.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3wheiizzd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3wcxjpfaq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yghpocyb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3adsdaysk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sykcovxw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tmtsfvns.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xmwnzbrx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gbtvynku.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3qaredcna.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cxslwxdw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gabzldgy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nwdqvczk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3opxpzxlt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ngkcovud.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3cgbyftaj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gxewkwue.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3iiryvylh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3lkwgiott.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3fyuvuzvq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3hfziqymf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3wkopztdg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3hbqubcae.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3domhvmgp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3uffmuzyf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3eqdczqwc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nsbvzbms.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ivrldbwg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3gbjybtqk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3weixnjbg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3vjcfuuew.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3cziqdcdm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3omlpgwvz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ltixlduc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jpwnqoab.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3bmkakfuw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3mibyrgzy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3etlaatvu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3owuhepee.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3nwkexjej.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3mqqjsspp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3piwlwnwr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3hjtcwpan.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3emhloxgl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3eshkdjwk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3vndpgrxi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rvtvglcr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3umqcejid.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3comkqyhm.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3odagmftu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ttefcrbc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3pjvarput.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3nyzwhbvk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lqutmfgv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3biwsxtlo.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3crnjpzrb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ndmqkoyt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3vbcomrtt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3avcqgfxs.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ndmchxkb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3vkpftpgq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ijmmuhwo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3iwoydmur.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ddljkwkl.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ylxozavj.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ymlmrcnp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ziwetvdr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3pecryeah.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wexxtmxr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tmshltpi.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3psesjjio.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gblhopvx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3perrbavu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tqdailmu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rcecnwqt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yvzktost.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3jsarntia.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3cidwsdqe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ajfjrgkc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wbpshodk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3vtdblznm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3poznzssk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3isuvjxvl.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3vlwdociu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3exjcjtxw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ugimnrnp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3txsdacba.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3maqroufx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vhofrqzn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3knyysbbh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ngmnrgky.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wjjhqvce.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ctmcyqfk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3bfxdywbq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3chudqhsy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3yojvjytx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xqrnlhnz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hluzupfh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3frmnbjnv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3glqngyek.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3wdtvjqkw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3zwuhcusf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3otqosrkx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3xiqnsakq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3hphvxcch.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hgegdypq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3syukvlpy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3gcddqyuz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3czzxhdbs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3acnvzdqp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lcpzeapf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zxblljse.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3yjhvzlwz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3arzhgwek.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lusyfsbi.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sdgxhlli.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nvhgzmje.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3afacmzre.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vtmtrwin.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3illkfaom.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hcceinba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gsasxkbf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3zxpykkiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwsxaymf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3owlcftwg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3kezjmwfe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wrnjievi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ndntryiw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3xpayeoxp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3lpzvywkf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3zuwbvwih.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zynogwjj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qtxvprxq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3hsqnknga.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ctdiabqi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lwhnrotk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jlhnchmm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3smxbfkap.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zqvuswwo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ynszenlz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xmnsmflq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3yadwnmts.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dlrraizl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3iapwyrkg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kkdemdwe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fhrsuymw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wesgwdmv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ifgsjqzh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jdgbnvtq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3xyojvime.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3awaorhry.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3yrvufmsk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bqqndyef.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3fxfzzlqq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3nfyidkas.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3eodjdjam.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lrdaxnww.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3gxmkgzzu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3qriafyqv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mxqdcdrw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3mtahdhem.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ojgzfwod.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3egbwxlxi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3azgmrtan.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oudglxhp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uxyclnei.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3twqpkniv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3imfgyslo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pmneybns.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3kzregzds.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lsgiuxtl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3hkakcoaz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3igvcabip.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kkshfnqv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sftgnovc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qcfbvneh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oepzxlxv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fytmtead.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3raomvyyg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3brqkdyfr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gnamwkan.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3inagaosi.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3owuesihb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ueqihvlf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3aimfsgpg.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3wmlnxvoq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3bycyglft.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3kapndbfc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3oyyztlre.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3dllmyxzu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uaskfham.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3imxuavyz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vsevwmxc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3oiundrvy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3oqlvmpvm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xdojnzjc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3dfjdoxgb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ppjaseud.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kqmfigsh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xlgffgdi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ywxnajhb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pnzhsfod.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3uscajnrf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3osxzjhth.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3voirxayu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3oszqvoea.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dcrvfuhz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3gbellksi.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rkxvwgxl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lxucgtfv.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xlbqrtwv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tgvimrnz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ldjvgwxf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3shkkfpyn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hjrkmlsg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dqjivinb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3npguvlxe.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3okzgfabd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xngaibin.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wxhvgpup.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3cvplvifx.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3axejilpj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3niqtxltw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3nmkzddoc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ipvuhszj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3qslkizwt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3sddxtfom.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mvuxxknn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3bywpgwsb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3sfmcyrtj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wowswzmm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3kbzurdrp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3azqbzrtx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3odvsscvx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ukiutzbb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vxhswlbq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fobtiwsu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhlmqbom.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xvciceit.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3awwbxdgd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yacycxfo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3xqnykowy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3pyjwprbp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3sjqiulpf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3twvnxiwf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eansvftt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fevdqvvu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3nujegnwz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3gyebmfug.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bdyjfgtk.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3gaewjkoj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3gkxjvhtb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qizaslgt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3dzbzwqcg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3bttvkbau.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3iflqfxqu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3cvizhlxa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3jhpodpbm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3sqwqyfsr.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3txwegxmj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3sdserkqy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3xcurkzfk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zwzpjxoe.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3omuzvyfz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3eaxoynqz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3dwlyyzhb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ugfjgndb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3kaypmphn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3xvsrsyvv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3imyrtzvt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ytwefedq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3bjowryya.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3kpmingwt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tzaafdve.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3yqylexac.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3dyeajzxk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3agjtvaxq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3wvdjxwnx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ezkpfida.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3zbtmidcj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rzzbksqd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wdirpjgd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yeskzvon.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ulmvgyjy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3wstdeedi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xnupjywu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3qsswcshz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3gdkhpqsc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3duzghury.html


<!-- 参考信息 -->