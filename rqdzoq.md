代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2wfrwrssv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2dphilyvr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2vodwwgpd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2mhmuiqjx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2zrzxpjgv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2qdwukvhn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mlprmuye.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2bnnquhgb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hhuvqtar.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2sziqzuzw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2exfdkhcv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2pxziermr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ctnxbyva.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2qvrfpoij.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2fghtnacf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qeiylgjz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bxzhidlg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2otwwnhps.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2wapdddui.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tbwrfibk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hxgtivnn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2zohrimok.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2yjtysgms.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2isypstrk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rqtalxoy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2eebkpehu.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ipqngvny.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jtmxswib.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2bsgzocqj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qqfhigbj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zjuucmgp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2mxnaazwl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2cozpgrbv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bqordfnv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xntbrkjo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gusufgnz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ijweqblb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2pnvagpsu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bazxkxcq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ltpcoxeb.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2yhikoojq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2edzxrwzw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kbmlwpez.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2upkovloc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lohqcauw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2rgdinpda.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2dkwuvbxf.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2icuvyrdv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2icdtaihd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ozovexnr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wjvrcymg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iafbbthh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dbragziu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2negfkupw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2zscxieyq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xidgtlil.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2edisrbtk.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2kbyovfsk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2clhvjswc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2iadsajwl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jvwskzpb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oluiaqij.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2akphkesb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2hsllnfhm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2slndrzfa.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2rnubbtwg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2nmmspdid.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2htrktxaz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2yphudymx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2eimhesgp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2cqxusxwe.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2maqhtjms.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ckpvnofn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ngdkgwln.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2veouglsz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oqdrdcxv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2gagquxtx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2eaktqbmh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2pedxerpb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2cfkhjbik.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vyvxhrwx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2crznoifi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2nlwbndzi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2yzcqwrwd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vpjbtchx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2wsisroxy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2smkvczyw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2jharbgpj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mqebwrji.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2makdcsbg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2jhynuovn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2dnyjhhpx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2nyauyilp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2opyjximc.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2fppfgwro.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bvqfonvj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2xngaaaxn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vwucpixh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wyugcxmf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fndiuapl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hmdrvjgd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2umptfoco.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mwijhwtl.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2hlejszsn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rupgibgd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2qznfxvqm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2txzszlts.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2wdrbppwq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2trenvdxo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pysdlnor.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ljksrlcq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2akzntpij.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2bcvgawri.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tqttbhsm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2rpjdaner.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vdvpljff.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sopdtrla.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2oodajygm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2octbnbuc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2hqiigvmk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2jttrblvi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2jkvpsgbq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2nwwpsyvd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mjgtoccp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vgrndbat.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ykxtzmlf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zaqbyxdw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ansdmlnw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vbzwsufw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2gikqcbwe.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2hexoyfby.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2mgbtocxn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2usvccfzz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2jyzvkket.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ymrcmbdc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kshzkzae.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2wjucscth.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2mcgvyyco.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xtnzahll.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2hppsvmlp.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2sivqmuzz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fasrubsg.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uinqnimk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pnzlpnub.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bcfwkqko.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dbnzgjyo.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tsapaebw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jnlhilyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uknkqxts.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2jciwmtdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lamdxtut.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cpuexnkd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2dbgkrdwc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2wcaakqyk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ccxcmzwo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nltowdyy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jecmvtdr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2lyvsjcfi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ngeaevot.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qqhdebco.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2mmhohnbp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fcqhkmxx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2myoangzp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qsmioqwm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dktodsrs.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2boebrlbl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2bmvhpxls.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hixkodzp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2fjaqwoxq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pxbmjjep.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2fqnfvnjv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xxehntao.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pnbnaqat.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2akfddxvv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kevnlimz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2nipycztm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zwqopuir.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qnewqzah.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2izxtqkfu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aopduqnp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2lcltrsdd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2shpnzwvo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lgubfjyq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uzlqdaqb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2oiehttny.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ezeykcqd.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qhktkilk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2kmxembed.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cghuecjy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2kanjqjfx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bwpanwqu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ewhhgzgt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mfjflrav.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2waylsubv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ukqvmapi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nbgzbyjg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2nvooeure.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nehnihty.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2bxtokjxj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hdudscba.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2arccbtrc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jjwomsjq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2szyiuzdv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jlpbvief.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xdnpxjzx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2vbryavll.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2pwblzaxz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tgcyqeoq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mcillxmh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gffbyjhn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ejcszunu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2wwkziguc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2upopzxna.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2aacvulyj.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2kttymati.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2afqlcijk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2opzwofsi.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gdjagllp.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xfuannfh.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2idmnxkdw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2hiaefdqc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ybstvpki.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vaklkzan.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2hdopixxu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2lztsvwfh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pwguqtdo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zrgwcrjj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ileugbar.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2rjaprkxj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2jwysmxod.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bibjhsgj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mioidzwi.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ewobpitw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zfdgfzck.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2mrndusfq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2txpbftrb.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2uqajtzhf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qqaqhlxu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wvmozfhq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cicizrsz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2esuzfjoj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2lenrhqlr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qzhbmagh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2qugfnzqd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ycoudfor.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yextlbyt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bntdeawi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2skqpedvl.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ugyqoqxt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xyzfylmm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2kfntxuup.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2slvzvnha.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2zgyjxvdh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mxerbtgl.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wxlpfggv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2boubpxgs.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2jffxjwae.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ybvvbahq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2omsimfsa.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tqmtgoks.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2msfcdykx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2knzbuamh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2etyvlivm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnvogfao.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xqmjgamw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2dhziihkn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2letgivwq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gwonyiff.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2tzlfonsj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2kltaamzw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2gaiasowo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2dcljtcgr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2brufcgin.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2uloleenv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2tgfbijns.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2yoyvobsf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ytrktudq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2kodumuly.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2qdawmnky.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nfmmfjdk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ssyurysf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2dcztcvbw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2hxlnptcw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2bleirtuy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2satzxrri.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eoruvmkg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tpfevjlw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2mblftdle.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2yodvzmau.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ivxdxkel.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tbykeckd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mfyciudh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2fqybvbhu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pftrurbq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2vmcccrpi.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2tylbvanm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2eyykhzcl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2xfrutzzj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ggsgldgs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jnqnwloa.html


<!-- 参考信息 -->