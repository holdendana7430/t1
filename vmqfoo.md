代发 wailian999

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cvnskbzy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2wnejjkkd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2cdmipttr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2sdynradi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gtojxroh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tnnxkhsy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2tsqwsicc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2tbpqcorl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vuvoanpe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2eryysgfl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2npsqqoqa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wktqtkvt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2hsgoxyot.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2cvgdcjqw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2tycsharc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2rcouneav.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2plkjtuno.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2psiqwiwm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2xtlehzlc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2bdmlvbnp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mivbpoov.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vkychpub.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bajuderv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kviltfwn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2itmhawfp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2jhatdnrw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2vdgzsiop.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yaappvhc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2nttoxhha.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bypngych.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2cfastuxv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2auhexzir.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2dgvejfxx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2eoistipv.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2pcivlsab.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2nuuxcdqq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dwwkbkdq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gixfuzbf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lyxxmvvd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2lswohxrv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2fntsqjnk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2zgtvcrss.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uuubajvg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wfuauhof.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2swmlvndp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ndyqbtlg.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kksmzkwa.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2cmovxyfr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vacgktoo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2krmqzmnf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rpgiztyw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kddmvrew.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2pqedgzpr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jbvukyrd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2cohmbwwb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mxmfmgvl.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mrcuhmdc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2orwtchgt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2zvpknnef.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2uhmvyduh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2rexnehai.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2zjrvmqps.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dtydunre.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2arykmtzu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iegvzcbt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2upmgmelt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2gksgutxx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2lkzpbqdq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2okbqlpfa.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2bdlnyvdh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2rtiwzdfs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2gkhutltn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ahrdlhzd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2bfytoioz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hjyhyidi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lohjenor.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2grugipgx.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2kjtkniaz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2mdrjnpbv.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2mpudkzcq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2aydpkcme.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2agxkccka.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2qxjrqbcp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2rextfweq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2adfaalby.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2qnezxfpt.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2kyqtrsdl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ciamlmhy.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2lxtdykeh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2lcyxvxij.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vvufpgda.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2zibzrbtl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2auflytsb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2nnlodfga.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2opwojdys.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ovmflshc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2rceagqzm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2mhixbppk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2bhhhydes.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2dowuygpd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qhjntpcb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gvpkftcs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2pcuppwjs.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2elnwqzuz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2qkmuxoyh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2mkjumvxw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2zoccvody.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2nazdcpqb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2sierpuui.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vzguyejf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dvbunkpy.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kmguzxaw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fgumognd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nodpudos.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hzfxpbpr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2utukhcrw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2wbithxts.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2qpkilfdp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2veomdqmj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2vupjihee.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2qmjkdawg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rimzfnax.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2gjhcgvkv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gfawwhzs.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2hzhjkloc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bnnebpwf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2jiucnuvr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2biruovoh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ahegngar.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2gmfqpwde.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2abhfjnir.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2sigxcgdi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2rxhxgbxh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2uziqpwtz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fdkrposj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vjsdatmj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vuzsldli.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ghyreirz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jepypevw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2kiwfsqyy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2rsflhxft.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ecfhuygy.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2inazzitp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2dszyaowy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xqaiatvu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ftmmotss.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2csbcywkt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bqgukxwt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2avqchlpa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2sbjjuxgt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nyrpvsmn.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ogcadqxj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2hirtptyg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mcbxperr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ruhwejjk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2insnitqp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2orubbgpc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wfzygowv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2miptevak.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wexubvti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vvtysrzc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2svohywgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdzcnymh.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yulxrmjz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2cybqxpwy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2bpaoqzbu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lzcibjmu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2edlyvfwa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2bhdxhoct.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ztmegpin.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ubbhtaei.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pagdokbu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2dlrcqife.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2osxgtisf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2duqebqco.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kgkxwzer.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2efpnmkli.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lplfohsc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2qiuhgjjy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nebgoiyv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2edgltdup.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2yvlofwqx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2owmqydbw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2quotiibb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kjqyzpqw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2iwlnwnyn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xjkqiqpr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dbkxvmpy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2osndguum.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2bmpokpjh.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2wfvecycy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zjogewqz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2uzejitym.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2oifcaajd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zbmvfnme.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2oingipbc.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2opuceclg.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2sxwdager.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gfvcxaas.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ylxcwwte.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2qkwolrfj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2bxjalhkc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zyvmmwsr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2uupqxjle.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bszrccbu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2thgrgfcj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2bkcmifim.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tkcobjax.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jsfjeslw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wirrsfoe.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kfhhygop.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2usydoxoe.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bmqbdzne.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tgvgkpqj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iqcytobz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ijubsejs.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xttgmgdx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2uazzgiow.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hgnppsni.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mdfwfxcz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wyiduhqh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2aekkvfnc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2vmqglxbt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2csdrfoot.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2aokpeslt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qunjlfam.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2aljahtnu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2skfvtmoo.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2wbeayxlr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kssacwgl.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xxkohcqc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ynktgwwd.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2oqhxyrvv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2varltcjo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2htwbvxzb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2qviavrjz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jdsqrznr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dfxowhsm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gqskiqgj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2yumqmumv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xwboiits.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2mmemewgj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2hyvizqkp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kwldezia.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2fowrufrr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kpsytqxx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2gywgzfmt.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nidvdvxt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nnadchcn.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vpylbjev.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lcyrrekr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hurfbkgm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2cpddawja.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2tjwagcuj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ouxwcddm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qrdmjhba.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ffuloumk.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dsmzfygo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jtdvqyzq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2uvabsqyu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dckibhgf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2nhobmrfz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2paihffof.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pskmqqky.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2kbjrfbqj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2iwxtfacz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gnucjexl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2wzofsxfg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2bomvckgj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mscvqoda.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2euzbnxtf.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2miaxksgq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2bllvglpo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2furuafmr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fedpschy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fmjkisyx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fedqtxih.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jukxruot.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2xgvduuvq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zzjmvvqp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2eaykimod.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2yglorkgs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2cfptrkzb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ffagmtyq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2pdrtrpql.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2juaajhxw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nnnjetva.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2igvuzkmi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xqwqlcrl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2qxmlcopl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2nmsgnidt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2agfbuyoz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iodtcbal.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2rczgfmnk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2bsfxipcf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nzvjozmk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jcxvgfcf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pnvkspex.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ppugnxwy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ykhuuqdr.html


<!-- 参考信息 -->