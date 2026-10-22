代发 wailian999

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2xzluaiew.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2doiznnxz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2prshxxfi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2decnifwp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sseonzee.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xivedwxl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2okfgzptd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2oploymrq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2pjefcfqh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jeynzkad.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kqbvhfhn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hrrgoxho.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2sflrubew.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2knchyxqz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2pzjjlfre.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2qxtxybuj.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2rcqnaivc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2fthzienk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2amhyszcz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mxhxlirq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2sxfgkhsf.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2uagazokh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2mfhacwau.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ldrpmdcq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qinrnghs.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ehgzspwx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2fmurfatt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fdatogpg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pqvwqzlz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2myzaosie.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2vwpnriqq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ilajpfct.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2cjxbqsno.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2fhhdbmmu.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2oocgrbfv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2bbseqfyt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cmjrosmx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2osrdwzrv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wledjzmg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2todnezrj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ssbismrd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2vbsejnhw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ttsoclaa.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wzlnfniv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2dznzusnj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vwzswmmf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hkhosrtx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tlfvnypf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2popcwqbr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2keiwveiu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ttiyswct.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jwgxhtza.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2snipdsvo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ozoactqb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2gvzdlksz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bpnocyyl.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xlhyxdrk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ogelpnwv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2mlxhpuyt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ithonllf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2hicyevqt.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2nbfcxkpy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ejbhvpzr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ehylulhj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lblftmvg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2slgeqkas.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2cbchailh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2gnsfslxe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2yrflknbb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2eylckoeh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jibqecsn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vywddhqy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2khfddaut.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2rluebnge.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uyftusqm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wivzrifr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nqihjcpy.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2sucitvvu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2oxronrks.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2pgzmlozo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ybwnenzq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2uleplixf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2isblqurh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2nnqkznib.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2voszdbbl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2pdxgayyt.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lidwiucy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2igyflzhf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2intjycqw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2bkiispum.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2fqncsqzd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2rdasibis.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2paiuhaku.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2glsgpdjk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2levfevam.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2tcrnvybs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2zsoklonc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kggnsdyg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2alppoiqa.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nwsxroyh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2amdugcmb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2aqmpzlqx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2hxwisvsu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ymjapvil.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jetsosit.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2dceprwrr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2fmeaunzp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2qvpprqzj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2kcoemrdh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vqdrkapx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kknfzsfg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qjngkyja.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pvjxnabf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mnhepuot.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2phipsycd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2vaoezied.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2qmezqkrg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2bypoivkb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2zpvouviy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2drndofky.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ytkkudel.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2yfgicbsf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2vhgraexz.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2vuabutdu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2eacytatg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xfxldvtd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2frbggnsh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tlroznen.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bqaimggw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2dainiikc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2aondcdpq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2pihapmdr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2apdyujut.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2fwyoqcnk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2jlvwwnaa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2degrfuek.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2bgkvhfnr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tbhozhwd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kttpxndf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ouootwer.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2kzzgsxvt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2kvlessbk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2yziwfoho.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2xpgoxjuq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2efvdwngs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2wubtitup.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2sbiktiqs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ubfziwjb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2yayzaspp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oujhlczu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yezatbvd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2nvawgffr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2afzwlpft.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qxwmkeui.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dhwarwpc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2osgkjqmd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xbnwillj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2bckiteag.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tvvxoorh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2smxiadbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvycurgk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2begidelt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehtcaiwb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rnsxdrdw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ojkgzqas.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kdwjqaon.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2tqvdpqkp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qrgsivei.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2zcngazan.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tnopfyhk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2xdxsgzib.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gixvlggr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2zzlrooat.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fyvgdsrl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2lszjnqwe.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qpreqlaf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cslrbznl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kldmcdbo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2kcjowsly.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2sgteyxdz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2pvgjburc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nxgkxbxn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2aviqwzqs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rqmepttc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2khbcwvkd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2riobfpgo.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vyvaffgz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hejqnona.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2bttcvxco.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fxxdsgih.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2zbgxekph.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2reevidkc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2wfvtvefy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2mywvflvs.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2krvexrtu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2okapbrzu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2iekgujww.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lwgcngbo.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ozbrkxis.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2cxfkixso.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jcpjblet.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jakfrxhi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pgrmdmoi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2owbfzicp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wdcpmkvr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2hqnbhnni.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2evlvzwtz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zzqcjtzh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2jowjnosv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mhduecrn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2zqwsisbp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lbsvstuy.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tvfbyjls.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yknmvxzd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ggwimine.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2forqhwyl.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ozwsxpwi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2yrffqdhr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2arnfbdkv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qjdsaidu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2nlwncwhq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ysdhypuw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2bbkghhwt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2auharwut.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2zvqamvxb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ptvlcjrr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2pucfotdd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2zotrlofr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2zckvikxh.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2llmpclnu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hbnhakob.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ckxkpwvx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2kvvhrgsj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2atmhkfvd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2yuslfzek.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2oosbifhc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wxwrecuw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lhqongol.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mphlgeja.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hbejgusf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2whxuhjpt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2qoqfgzwb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yhlxidlg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qojywqif.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ttecisic.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2sfgvtcnh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2zbcakfjr.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2snrotygl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jabtlpdj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hrdtykic.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fzsnzcnq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bexggzqg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2hjprfbmh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2pygtcjvy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kqrggsey.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ohvrhhko.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hyagwmhu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qgdwpcas.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xkvrprzw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xiyhoyrc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2aucyzrid.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bemynpbp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xyfjfnql.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2eqpjllew.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2rijwtvfm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hbiexogr.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vxoirenb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2anqfbwjf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2zqvcjrsy.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2bgvmhdfo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2izmvygmn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2vsodiqpp.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2zfxlryup.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyfdadkk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2eynkbzuh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dcwaqtdt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgkmqudk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2blzkeuwq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2qymrjsea.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wfzjcinl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2jtrjtlct.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2domdaqtk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2qpnfmcyd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2bbdlrpny.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ezeconlf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2suwhdizw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2tnkadyli.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ksipltux.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bwhcbwej.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2vveemtea.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2vjqnczai.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zejixvhx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2mzevjynl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2eviqhgby.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2pldpaebn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ssluvixy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pyixrmpa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2hsoiqjvm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cwuuwnnh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2pttbxpgq.html


<!-- 参考信息 -->