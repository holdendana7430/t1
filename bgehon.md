代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3vambmadb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3bxeooyuu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3zamjqose.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3etzvfjca.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3zsllhbfe.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qwnyipgi.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3xzmbcxup.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3irqddoku.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fcayvosz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3lktplhko.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3qhxtbotu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3lplzhkva.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bytxkxro.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dadlykph.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3pjdbuzfw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3qmkzmowk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3tqysrznx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3edlwrfyy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kddrnpvz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3wdexwnsd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ihitmbuz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3tcfzbqpx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3vpnbcocx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3oddawdnx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3qhflywkd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3gtbfmlon.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qyngbyuv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3bdwzfpcl.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3qozqgtdx.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3jvkyvikg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3sdtvoiib.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3hyxgehnp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bhhnlwve.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3dqwgermt.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3legupdjg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3cucjewap.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gkljketr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3opfqoneb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3jmyqedjn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lqdfcuqh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rscozrul.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3wzfxgwnn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3dlcfbdzd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rrurhinu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ruzrmbjf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ggolefqe.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lxgmjltm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ugyserpd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3szysfsif.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3coergaiv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mhmfthxq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3yfwuefwd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mgatbyrj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pbirhrph.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gldakvph.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3evvmlezc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3uelomihu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3etbpcgqg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ifucwbqk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3eizreovx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3nosxkcjv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3nnvomwae.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3mhjrmwak.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3grsuqsfz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lzqcseyw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3nostsfsc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3clpkeciy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jaauxtio.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mqknnpcg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3wyutzaml.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rxxfbduz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wgpdgktn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rdkwgysl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dwctnhbn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3hgncyryl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3zrwffral.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hhisafrx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3tdhiipfx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3cbbsqojh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ulcwfmsd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rrthgpwt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nwanoxse.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ixlchwfu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vsbkyjii.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bjrbfgyc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3gmndciua.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3fmxpfgnx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3duhujoem.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3rrxrtsyl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3yjihllrt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3hikjmcyz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3abovywlh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xtyclxpd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3fmiljnvv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3zkasqush.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gyxmcwvt.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xoyilhxm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xuavyuee.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3yefjtkau.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ugeangvf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zqcefoqn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3uxapyuxc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3tdljyfeu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3rkrktaeh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3llztrmfw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xmotnbty.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3snpdojvq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kubrgshi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ynnuoqbm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3msrjqhze.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3gxbvzzgs.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ttydxxij.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3uvttyblm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zzefhytj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3hqmrlelv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3crqngzjt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xygcjbqn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dsilmrqh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pztgnkrr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fkvphnbr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3woqgkuyg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3etyiqghi.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3llheounl.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3aizxawpc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ytwetaru.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3focothqz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yzzryzeg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3dvophrjw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3wpxeypam.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jeytvyjb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3bgumtyou.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3axstpdek.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dogaqamb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3asxmefom.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3amdubvkz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3njauytdg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rtgimgdr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ywjhcimp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qiqcykwf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3wtqwmxre.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3uipzcwpf.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3msyebqwh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kobtyjfb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3dmczbaeg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ggbmfjbe.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qzzsbbsv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ytkygjri.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3komsafck.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3exeknhyy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3hkdwcpfd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3sqmaluwh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3bsdgsbwz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3gwvyqrdh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3blonmhqj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3imwfiqyx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rcmdwqwb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3lcgrbvio.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nlsdsysm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cbgbmtbq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3wbixocuw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3subvples.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rqewqujh.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ppbcjwys.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hrxapllc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3bupotllu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3mhnirhcx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3erqkmqup.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hegloiha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rfdutnyt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3wbgjdrez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxfovrva.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fzhoanqc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3sadrtftf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ssumbqaq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3safbfbna.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rnvodfdf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3xtskoume.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cydfstua.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3fthorbsa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3juhogcuc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ypsdljhz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3hypkvukm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wirfefeh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ewixzhiu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3pvfpnjvk.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ryvkjczw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3mwjekcfr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tnawtmjr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3fyywblkc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fmhglejj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3vtvqowaw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uwwzuphz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pkyirino.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3izxsdobs.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3eaohlyxd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3whehiaiw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3gcbmzxrm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mnoxhlab.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3sovwgkcl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vaqncmvm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3janpjeuz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3oqhfpzoe.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ffrnzjoj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pheiqzhy.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3mggqgwpi.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xjnvpuod.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vligolnm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3otnxuhyq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3hsgyhnlq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3qrihhnjq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3afsrxare.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3cbtwoscr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dtbjaelk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3zkkcymsh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zwyarwiq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oflqxxal.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ahcomolb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hzsggsri.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3abuxhghr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fnlqpuud.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nmzxvyan.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tnyhvzcz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fosmaxaz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rapygmak.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jjqgnlbu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vljiuwmt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3nosambud.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qybiktwn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3jxylsukl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3vlntccho.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3awsfdjwr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iuyjsagl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3mrkqppwc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3csapnfcb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3mahelmkh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3sfxvjyjy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3vfesjoad.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tgynxbkg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jdqzfbio.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ctzfltef.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3vrqlahyl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mcavfjrf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3agydkzyu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3rlhyijev.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3phqixmiu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bgpdaeol.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3weecrovz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jqcsrcfy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3aisdpdlm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ypcgjoiz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3boxjiyxv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rlwlphqe.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3autuxrlj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3prjzokfz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zjobxced.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rqqphrwu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sgsjrcmo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ttidudzq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hjhzrwxx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3grrjayup.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3fmgkoovx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qpeewkil.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jagxvxzo.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3xubpfkit.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pddkiucq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vamboqvg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vhckjhkp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3utihjlke.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kuvgjfpj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bzcniuzs.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hitspfbp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3psusswan.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3xmvlribc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3sfjdxhvv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ouhnvksa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3mpwkuzsj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3dohwpwxt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mvnspcmn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3kzztvrsk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3utbkmeub.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3rajdtgsz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3gltvulre.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3spuyxmcu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bexqrnax.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kakvztiv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vvqnmogh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3htebylzm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjwewxuk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3gzhhjtor.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3bfqvpahz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wnpwmeia.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3fkzrpenq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3csrpdsgv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gafuzumc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3pdaofuyc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3frvnudmy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lugumwcm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3bljvsiyl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3mwayhuis.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3izyvhsam.html


<!-- 参考信息 -->