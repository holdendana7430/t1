代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ogcmdehq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jcibveyf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lsejeghb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ieffoaii.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2czxjlkpe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2nwbxyoyh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2effxiygt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xzxoeldk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2uimnhlzz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2qbuardno.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2qpuixbmf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2frnylcgb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sawiakap.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ydejetfa.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2cogghjiv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ejhqacuk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2vopqbvdv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2mjlfyfdp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ynezulwj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2liutuyxk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rpwamnum.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2inoeguiw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2bucnfauf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jfwxxxhx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wzhimjqe.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2dvnugutq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2aejtictx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xihuuqog.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2qvligifu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2yvfwjaif.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zxhbvszs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2dmvpjzlt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2iwigfqge.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2hbfyyvsy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jfemmbol.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2igdoxtbe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xhajrcdc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lfvqnacp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wctjulep.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hgxbypuj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yylehith.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2irhrqcqi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yizfcfyr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fukcfrfu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2tuyktlib.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vmmzepuv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2avavppai.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qgtdwjvn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xydmqeqk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2uycqllsz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2lffhxehn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2cprhbidf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2egzdgczp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2rpdhjxtk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hlyjsspv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dnwodukv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uhewpgzb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2idovcuif.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2vofomtlm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2xewyxgcx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qjlayhmj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2aexhyxnh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2sahrvksj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2leojsmxe.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2fmustemx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zewzrjiq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ditnircv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iiiihygc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zczmuykz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2erxoinjc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2wbihqlum.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2pqcepafw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2tuztxftg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ajoliiub.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2lghzpvff.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2bddbsnzh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ccvehjqa.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ezaiprav.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2oszsntzk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xkppedsm.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ohxqgyxf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjuoeznq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2bnsbdann.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2xvsbpbdy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nkkytrrq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2umomepvi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2jncfesim.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2duorcany.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2onnvmbxu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2oqmqcsfc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2jzhihmck.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hsrflwfy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ubjnhwok.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2busrhjzv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2asbiougs.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2yovketev.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2dqxjlzom.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2whyjfuym.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2jitxlvxd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ojrwfrcq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fvuwhemz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2agrdgcln.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iahhaqdp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mdbtkjmx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ybbckaul.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dfxpzhrx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ahdhqqbx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2tvipqylj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jmfxpmyi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2vxxcaipb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2dvufbmbo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2kxweaiie.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2gbvoisyr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2hxolzltw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2pnquvntn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2cmrkscxu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2usvvkavx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zxdhuajo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2pdjlqoqx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lnmfydft.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2grvaemru.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2txgiiofs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2skofugix.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2hjwhukud.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2cqrurbpm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ciplnfxa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2txugodjx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mdqwrjcw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2tyotopei.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iumwsizx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2rrfwtxpp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2mzffuvlo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fogeaghx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2vhpivgjm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vdftgzql.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2nigkmiko.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2bmxvqvuo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2vtibsrax.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2bhntpxvs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2yokjeavt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2vnrwwbbx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qkvlgsej.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hcsbrowx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oximidse.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kgxnxluk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2oqirustn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fgmcpony.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xiivtmip.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cftkerbo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cdrmdybj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vsqkiilm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vafywrze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzdwnkpi.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2wukhcsqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xesuxsvo.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2aimahzoa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2bkggjcfx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bwulnxso.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vqdzhgve.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ycnuzyuv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2uoormuvf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2kbscldin.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2tsltamii.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2thgaxjss.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2swspmipb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2subzkzzq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2dwykbezc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uqnnhodt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2syvsuilx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uzjqgnmt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zoarkrcx.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2czxrpsxf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2lcblhygl.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2mujetqgy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2vnziukme.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zvodszrg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yvcasgcr.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2aqqtjmhp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yosxryuh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fddnoykw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jfwanlis.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jryqzfbq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2mfmrtvkg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2renmmvkl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2rsyisbrx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2tnepwhlc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nqlkjdxo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lvwihvdx.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ywvigcma.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2denkmqrv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iibhftny.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2polvrtfp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2cwjkotsh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2axwbtuqr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sbraafto.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2seycgkae.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pgrxrlih.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2pkcvhmsr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2umaengmc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mgqdsrvn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2rjouxihb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qusmtsuk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2eyedezmm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wgxyaves.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sztnrtym.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qwueghbe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qsradmwr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lkmkxhpw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tanaurcm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2taozexni.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2sbaoggaf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fhyycure.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jngfkxsh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2oqimatty.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2jzkfafkl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2guthrgjs.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2yhrpwzux.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2lwcaokls.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2mvfvivfe.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2zyevwnks.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2nhazoisv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2oszkfclm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2imxnxiny.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ajacfwok.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2whluifsr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2alaqkplo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2iibhclbp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ynmbuxef.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2thyzetgu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2mkqodldg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2papwbtib.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wzhfvvxn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xtqdencx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2gxlfpgtc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2rqarwlap.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2tjiqnhjt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zogwdchw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xwsckbut.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ulrhzprs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kbqjhbqm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2otltksub.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tvndbrjp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bmxqwtep.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pvuojkyw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2zsgywjaq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2mtifobjr.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hofaujze.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mmchqqpm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ddrablso.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jkrfxhkg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nxvvldtf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2yndpjons.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2krrerlcz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hzxfehsi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hdxnkova.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hamjevyd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2dtijsdil.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cbcuegpf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gnynvfkn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2rywclpih.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2vcznracr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wsvlxugv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2fndjvghy.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2pkatdwqp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2tohfnsak.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2kqvyxhxr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kjmfzlxq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kmdlayjk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2msjxxumo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cjarcmat.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2evhbbflf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2eqtldnia.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2cnpglskj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2rojrlbdf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2zledhjsb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2rkkprsse.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2vpqgnlpo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zykfikrf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2bkqibnyf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2xqaohfat.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tjpeswuu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2bittdslr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fuwzuqxr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2fnmtkntf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2nsdoqitp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2rkxkqwsg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2crexylft.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eoiomwpn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2bdnhvmmo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2itjvmjfh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2iahztzge.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gfuxyqww.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2obzjyqzs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gpwkfros.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2upgehwyx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wswhcqxv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2bbwewwjt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2tohtilkd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2rvsgakly.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2vxastdoj.html


<!-- 参考信息 -->