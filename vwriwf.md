代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rgihzbkq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ndwpvcwn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ecarftmo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kkdpaelh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3fcuydgkj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3wawagsrp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3pexvydha.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3xgvlraju.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3xrqpfcnr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3lirrlcag.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ykjqhlju.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3lpgvwnpt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mzhphycg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kwdwdcho.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3dxauccty.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pobmtgcj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cdtwlddf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3iewfjffi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3wuexezer.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ddoenadx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xpmszajb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hipodykr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3bfaofssk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jjrwapzs.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wxslckou.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3cpoajdzw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3lgejentk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jnwrehhm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3klyfmjfn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wmgudxeu.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3assluhfm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iimlfmki.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3mnrltvjy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3jcpouwzw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bpfbxqzb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3umrlizyb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3gcvhvoeb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hnmynaie.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hgfvuyxw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3twaqtxbz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vxolhoqv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mclaqozb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wzdcxjjp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3imabqvrh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3alfpgceb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fglvienq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uvkimshn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3emofjkji.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3sbaybibz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3lfiamefq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3rknpfcgs.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3dfeqgiwc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dbjkpzba.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3hncpipuq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wodtlzyv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3latmynch.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mzfcptfj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qbjfxpvg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3tikbulsf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3fnljjnfa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3vxpkpyfm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3didwaakx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3dqfmygvp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ohpmuaug.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qkmzkzei.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3poeqrsay.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jogvvotb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3crrgrjod.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3uejgbply.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3payiajgk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ppsmbfdh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3fraspxkg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3luxrdjun.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3htvbymzv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ewfzfoup.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3vuqqcrsd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zmxuqnge.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3mfyivmli.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3taudzjdt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3czxrgqox.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3svzoelhn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3khvsdgob.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3dgpnshtq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3mencwwuc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nzvetrjc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3uyftlfye.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3zhqlfmlk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3pkznzzfv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ydwzgvob.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3paxoszgf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ikjgykep.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3qgojjkls.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ijnjkhzt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xktgekcs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3pemxhhiv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3cgomxgnf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ftlrtvxs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3rqoarkzu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ehouswvh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3hnigobxh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ggianrfd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uwqqvhyl.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fiitwhnk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gmnexlhm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bhunwepb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3crrlhqqu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3elbgbhbw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3tfpvzkzm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lknqnfee.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3dyfesrkw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ftwzhbjb.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3oafmewcg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3qksbpgga.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3tvsuhocj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3hdxbtcec.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wxoutxer.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ikqbkrys.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gpytylap.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3klwneeyj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3neqhqisy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hwnlzdkr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3gmboibje.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3srzdhtew.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3hovlitzw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3votfjdtv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3erwvxpfi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vrtmvppo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3gquouzik.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vqahawek.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tpbiicuv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kyarmxol.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3evkqqgrw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lokonuef.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3rjzwoalh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3oruwtnlk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ivtmilmt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3uqjbycjt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3rhfdbuey.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3jtvtfyct.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dlvmygje.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3zylrnwos.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wtgkfuia.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3gaorcvsl.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ghzvtpvs.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zikykmts.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vvycumyk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zyyuvnio.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3usowmatt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jsjpthdw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wfqjvgoa.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vvlmegjx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wactjkmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uzmwsbyz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jhkjixpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bskzrmho.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bshcxcfi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3yeezqkyt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3zhyaflil.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3loezcvpe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3mstpkaau.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3sospdilt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3awnxzswm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3wgcfdzdi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cvakwwzi.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3dfzlsbhd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mcqrakzr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3trlsdmpa.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hvvrhmtb.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yilfnnzu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aecbxpgb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3jfwbvucx.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3jdxijwkk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fetiotbp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mfmsvbbi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3uxmasukm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3njzucrsa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3slldnoxo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mmiqptyr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kuqaolrp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lgedrjpj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ozfdgopm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3skfrawvs.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3lqcgccen.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3soluavvo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3vpdvhifj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3tgbmfrjs.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3inbiilxe.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jjdknrtp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ttpldepm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3abrvcyjg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mfmzqyho.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3wqtjbqyj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bfqbjtmk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3xitxfjkw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vdmgxnvy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3xlnglpzy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jzgpxdux.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3kfhavhjm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lwaghxud.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vfwfjorn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3pefqanjj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vympdwaz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mhaewkwt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xtecwdiv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iribqned.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hyxuqkxg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nymltetw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sfyxkeor.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gtaomwgt.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3iirhysno.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3mytgipkk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3htlqjmaq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3sosqxpey.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3myjnsmce.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3bvoomhvz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3dctjloir.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3sigvawbj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3txqrzruz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3uhxhrfvk.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jdvccaie.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ecwstxza.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bkhomzuv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tkfguewp.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3eejrvcbl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ljpqnhul.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xrciudsi.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zrknhhvj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3fiogtrft.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ntolwunh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3odwxgyjw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3soavrmsj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3eyvabpta.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3juyzwxae.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3oyngewhr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tzbqnijj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kxrzvhlq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ruwtidzi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qecmvvnu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3bpwfatjc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bczhzczh.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3btrekslo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jqegvtub.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ofrtqsap.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3socvrlmk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3teuojulu.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3vocxmlvi.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3osyvygwt.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lwcserxv.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3elmlcorz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vuppimkw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3qcmtbpmc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zpkkanjt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wkyczzjy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dbhlucyw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rclxnepk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hrlbcvwk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ksmihqbb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ifreikyf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3itfizdcu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3oanaewbc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3tkvqdvgx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zzqwrkpx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3nkrfocct.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3yekdegfk.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3lajvaoug.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3plffefie.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kalnmvuo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3avqjakor.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pjwrtwyr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cryxepsr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3dteocvdh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qcvgvwds.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3qhruxqrn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3hkwpxmtp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rxlhzxxk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3joduqodw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zshvyuax.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ohkjjyvz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3njzngoqr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3daoinhjf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fmtnknfe.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3vgpdfkrg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3oqvbniae.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3xhphtkeh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ijuqnxml.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ihnhcmzd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3mcbosqzk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gmlsgpwk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oekbfgtx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ncgyzhqe.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3shvhsirs.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3mlzwrboo.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qyabmvkt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fzkdmraq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3oflhokep.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3lpvvugmg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3iffigsrx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lhmdylnv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3vtjftudy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3hkkxugvl.html


<!-- 参考信息 -->