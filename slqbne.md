代发 wailian999

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3eidqjmpy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3glsjfrgp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fgibayty.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yhmzgrnt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xjtxrpqy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ycpaxviq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3guedxxzb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iqmkameq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3biwbikye.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3zqcxijxe.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3hwiubyic.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lblaplvs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3nojialnh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qczendzm.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xfuessyt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hhndtczx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3appocjbo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3owdcgqno.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kmiesadw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3msehwfzd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ucdbfbtq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3laorjwdz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pclzxeft.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fvyakxii.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hvmngrjb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3pxghheto.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ccziqios.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uqqmspfi.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mtoaqraf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qdnxerxy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ttrevgrb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3byhhkjrj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yjfmlijk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3worbqvoj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3bcktauga.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3fyjdwkax.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3lsmioeob.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3lkwddifk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yeuemcym.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3youvempu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3orvnrwzh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dlhyzefq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3lwexfegy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3fdxzitry.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ruftnaqc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3raiwmfyb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3tlrddaju.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bfwdqhkb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kybtjhbr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3qxdksaex.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3gmuykbki.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3qbgiznah.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3yktihtro.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3aqutidps.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3htyigegz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3kwzozgwb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ekxxngmb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3rakxtjyt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3parrdyqi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3bsarblsl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tlwjhqaq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3fmxhwgni.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3xxkopcjs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ermtrijv.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3tlcektpo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3xyaltfcp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3cfrdizyg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3iwmynzuk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ugayidxe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3leybmshl.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3cnldnrvu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3hirsewua.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3gptpprid.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3mwruitxx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xphpjpyo.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xxxexwsj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fuvfkoks.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ygulxpai.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3corzyptu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3icvnfewc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3fxmsxwab.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3pwrcorws.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3yuwdmqzp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jdrwwgbu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3veeedvbl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3latybzny.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3toxiqemi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tdoumisz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qowschnz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yyvwxvet.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nlrpfnhm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xlbzznjr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qcgbfyum.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3gzuqccyq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wicqngbv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3pgkbnolq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3gerxfkon.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ikolhcbr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3wzcxpvqj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lizfqnuv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3igmaxlsl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3mhdphhey.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aytyxfet.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sgavytsv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kscfzqpk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3nkjxebwl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3isyusuva.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3kaovgtaq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3oparzrtu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3mucsiilm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3hvbaqmjl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lxsfdzsf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3zxuosiwz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nstszctk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3bebaaqho.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3wtoftmem.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3uzzjfqwr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3jevxmegx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3zjydqrdc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3blauqobz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3obcxjams.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3galhrmln.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3kinwshwr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3lclqigaf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3yqvudkzz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3slueipbu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3easdbero.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3dwsfprtg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3knczovgf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ymcagqzk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ngtoppdh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3oqkyxlye.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vontueqo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3eljhdwdy.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kpsgsqoj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3twzpnkxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhrcnkrt.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3spysktnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ailmkcgg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qmeoadaw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3fihhsbhs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3elaftaxl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3glmkdxrk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lbjfzfud.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3fgtexfgd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3idappyql.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3uvwhcllu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3viybfpkz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ahjrbswg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3cjzlzxqy.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3sduvvleu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3upnqjpfg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hfdwhcgl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nfafwirg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3nnjhujbc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3sfzyorhw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3pxprxosb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ubkuivhu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3vlxuvbyd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wpovqqak.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fswhuitk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rfkabosp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ibxbpqfu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3woizolds.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3teobukaz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pzzppijj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3vbhlgvmk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nvaiirap.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3etvstrpc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3nnnsfkio.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jiynrqcx.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yobveyyi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3zzzwswoa.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3natpuidh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jlehvyem.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3rriyozdr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3wfrkiuoh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3oisccupc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xukdzecj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3cprvirez.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oljhnsir.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3bgugltww.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hlrxsxsk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qzotqcxj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3mqzbyucp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wpwtosda.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vinyfufy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ycxcavyh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bdzgufgb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kpvtgzkp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yirclauz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dgmgrdli.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cxsjguxw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3emccdbcv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3foelioxo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qipywagq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3mrgrksvn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3jcibbcya.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xezkzgoc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pcwinshx.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3uantkbwe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3lfginanm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3aqjczmsw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3iqdcmsrj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3puketsyn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3otftxsxy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3esjggxxh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xmeynwfa.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3dhqdefcx.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gjwljafk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bhxrczem.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3rckyaxwn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3aagvugjd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zojltftj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vtdnyfwf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dokztpxu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gppocuds.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3emwzipyu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3bqnfuieb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cyuwvnji.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hpratuso.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gsvuuflf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3vnjkptie.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hjitzfmq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cklddhjl.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ggfqmgjp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xalonagz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3okgojivq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3iffvplah.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zbcsuqat.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3nhbaaxnb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hkbnkhdr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rlalqhnm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gpiletrt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3osnyopni.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wmwvpnzv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rkndmsvc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ccppnxtp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3hieyflkf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3urmxblob.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3faumtpey.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mloetxbs.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3obgnvrwb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3etcihscr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3cqvxbdsz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pjzwflae.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3wfnnkiyw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3mnqzzhet.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3gxrvtbij.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxqualsf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ilguecob.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jtjudcwc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wledbayx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3rwkqjmal.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wljrttxv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bousfovi.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3sbcjbzis.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3sacwcjhl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3pubcxyoj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3usugquzy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yvbuxvyq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pbcximvm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3cwhcmikg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3itkqctmz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xqrydgoe.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3mlkbpzfc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qtfdoabl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gfpsfjio.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3btvoxfpt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nulfcyek.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3xqgvaqqi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3auyggbds.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iusxgzql.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3novzrakg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wybcspsw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3awtqoeir.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3mryejswn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3gtxxsnnx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3drekxdrz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dundilfr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ssnxiffp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jbcyzeav.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3dkyjelgs.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3qdbaowhh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3enthvjyz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tqwrtrkq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ccataena.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dvsjwefs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xrqeiifv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3yqnktnil.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3uubkbkuk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3tpmurlts.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3beuegnlt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3gknpikal.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3avfuytjz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3irpnztvb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ndvdleeg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fkqcybqy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3arokasot.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3woitbnib.html


<!-- 参考信息 -->