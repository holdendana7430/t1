代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3pemipsoy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3njyklkce.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3swvxzxcj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3skttmodd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3jdaxdayj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3tyvsozcn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3bgdigcuw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3zgyduvww.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gkfuaymi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qkgvusaz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3tqhgpley.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3eazslcea.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3aekrbrak.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xulhoqah.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pbtlhyqp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3blqzkjuv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3esmtulpb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3odchjmsm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3vfbuaqyt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wnftdbvt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3xkyweslo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3wqtepkjo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3nwkzpuzb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3tiueuqhb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ctfowemg.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3khkpwuxu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jmoehngx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kfmebvrz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3tgtseswa.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3yxcblicc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3xjwsbtar.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jwscbjkf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nieornop.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ovvisuib.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3tojgbvtp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3byybhgsf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ybkrhxfj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3jaqwqtgb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3iwnmuxkq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3isgnlaom.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aouljfkd.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ptixwpsc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gjhpekoj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3jpbtotlb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ddlernlk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3pmatzzrg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lpxembhp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zyntiora.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kwibfylj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3idirtirc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qnnvmiby.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ufbvjfmd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3sxxteuqh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ucmubqgw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kxzwmbrh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3aijojctu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3enkyqrvm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dtpengfk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3kwswmwhq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qddlosbn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lzdzldqx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3oiwibqdm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3nmbfonsb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3lrhnhnec.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uypxkyjw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3gedqmbpf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kojvvndj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3opszzlfk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nigoywbb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gcnicoxz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3kmoapykp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3djvyeclo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ydlrrftg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3pijakgqw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3srksvfec.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zzfjnqsx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gjcrxwow.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fquebqwi.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3fwxsxyky.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xrhhsnky.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rsuwcpud.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ysudiqum.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3bornkics.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3cotkqshc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3mzbuwvei.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3bpphvgei.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3luvguzue.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ebbuoqyk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zkzngqjh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3gaxdtnon.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3wythuieu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tfhdlfcg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3hvooeanf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uspdjlma.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3saypiabb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3iqueojzw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3osppenur.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ojcvtget.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3imqkuaht.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ulyedhqo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3dzvebotk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ykqrpbed.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3cjlxjovc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nhjrcszz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zctzsqig.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3sbcxgfwq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3mmtsgjzt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3dxdsdefl.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3hkunkgwu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3igprfcbg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3wpuxjgmw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3chamsrls.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3bpxwjcqk.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mzzozllu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3atcprfwf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qinzpmdo.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bqosvtdo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lkjifulx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vlxekisk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3sbeyvsen.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3zvifhidh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ttlsdvfc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3wbvbvekz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3obzbnzzg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xutatkmg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3buyageld.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3vunxniwa.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3gpedoayb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3igzmwndz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ifjcbere.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3bqbrcyqd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xabpppvx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3szxigwbw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3lreedjsi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ebdnslbj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3dgvwpcky.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3dwuruuwc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ivktxvyq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3fzcdthap.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vlcjuvcj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tkmikdzc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ptxomqbw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gghmneie.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3dsflkrqz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3amevjdhf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3qehtabfg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3vjwuiyjw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3tykxbjfl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3popiswcg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uwzutzss.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vrkrqypa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cjsjwxyd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3gecrdlgj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3qzkdwmym.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3awwtccld.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3enmsvdwb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3jrtncjwj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rtzhzgmj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3umczjjff.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bloxftwm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3isgntwsz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cvyfktzm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bbofyuci.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gygskibi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgmkqpaf.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3nbsfibjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sehtojnz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mihpooji.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3vdkicxue.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3uplsklbh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rctydczs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zmuycvtn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3xyutrezb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ezqzqkhb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3zmxrygja.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bftorizq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nhcdjvdo.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zvhmaxgc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tyznbiml.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gopqxcyr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ztsoalwg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yrphruja.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3olqavikc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zrmltkqe.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yndyubdu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xbzwrceg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3kuecwblf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cnzqivld.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dixnnqch.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dpbwnmfr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kdzqoznp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ktfyvjux.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3nwskljtz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mpmrytis.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3yiqttzjz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3pkrejlxk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3eokhvasb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3zxzmfgiv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eavjfiyd.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nhjecrqt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3jggqvxgc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3okqhrhtg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pyzvruqy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3wckldaki.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nwnuwvxp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ynljkewe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wbgwrzuo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3zaczgdza.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3twldqpmq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xpsguzto.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uelmzodz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sbfkeknx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3mldscxar.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xrtcgpni.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3klwcjpdf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gritbfnu.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qatvuwag.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mzahepnr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3upxpanxp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nyogsvdf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qwagyfbm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3robecnen.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3nkkjpdjg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3psoieaht.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3bjrikocd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3hnsoeprd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3whltvsic.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3nxcieiji.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3opfmrrfd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3xxuadeaf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ccpcfntg.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3yeuqmvsr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ablcismh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cslzmsgz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vplasmhk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qlhcdedw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3leuzjibl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xhbrpkiy.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3fzqaphbk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3enmkdrzx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3oeoymwvz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ttdvybqf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lyeisfzc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mqgzpxuv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3uaxbbvkm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3xxfehdjc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3mlfavket.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yotptyhq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hppriogr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dxbkihif.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3yoigeawq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qjzieray.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fzdmrnyj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yenihqtx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ntwlfzuj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ugdmmmqc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3gbtnjmrq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3jiruxcho.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vdtxsejv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qtopclgk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fpfypfri.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3abfwmmox.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ycjiklce.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bejyifjf.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3czaprpqk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ghubuoen.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3nkdcwprr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qjrcvumy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3mxrcfppd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3smqutzxs.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bgwnziqp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3xsnzubhk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3uijtcngk.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xrsmiyru.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3nypaucmf.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ntlrnbho.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3hnakqojn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3cwiucajh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rpseknxl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzcnfdml.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgdsmylo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bnawsgly.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3xqvzhwdr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3awdxrtzt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3trzkznjq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3utsvneok.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3fmvpujdl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3avwjidai.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vbvazkvf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qgkejgav.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3iuaztlst.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3kdlhsqtn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rbwenhbc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3zjcygsrb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aythfili.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jchbzsff.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3rneexukp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ltdbuaga.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3iyrzbdhw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qqydqexn.html


<!-- 参考信息 -->