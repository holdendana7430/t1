代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3issszuwz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3hkjsnwpl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3sodgrexe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ngcympsz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3cihabrua.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3duxiydrm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qhwdojuy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3rfdrbfmo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3lhvkprcd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3wuzprwdi.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vjjmcxhc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3skzlvnjq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3nfhhdbge.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3lcaedpxf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3vqdftgdr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3crfyjwvn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3tcwtvfrd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ftwvefxi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3kciguwll.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oaxosagm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ioadynmg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3mmslrvya.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3qmjkwqip.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3exqxnnen.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3wubwvjcb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lpkirggs.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3guwfdryr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hihtwbtp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3fdhyxcub.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3yvtuefbi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tirwhnpv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3aakwfcnw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zxjqfirq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ajvomwcl.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zrkgvrll.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ankkjpkv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3uqvmcmic.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3pcalkxbb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3txsnbahb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rifgdfga.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ogsigzuh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jmrkgwge.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qdjethcf.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3djfhdnea.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vmowwqxm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3nwegieyh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3nzlonmbq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3pipbtvue.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3cjkqczhs.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3huysexof.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3edhhlphe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ulswynfw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rzwtxcgh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bemnhflw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ackhutao.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3lekdeoqh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3zosmzhjo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3bylvxfzo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dsbnnnpl.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wvpkickn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3muuxifiz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kmorwbze.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qjltjwuo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ftskpvkg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xvjvcwaw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3itxwcezm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3jlrsszhn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ciqnpoza.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nozowzdy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3sshaundy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3bnojjebo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3mazlaqvf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3qmwswopa.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3icfwriqs.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3cvghhtwe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3flwotyhy.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ihfurdbv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3tkkcdciq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3kypkeqmb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3uhlxsega.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qifnlian.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wwtkqiur.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ojphdoik.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3vixhpkvv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3oemxkixu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3qeyuifer.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3pmnnxgbg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3wyjebhwv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tkrpsimb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cdrwcloq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3inweuazo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3mtyjqyca.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3hwppgqfi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3yzundodx.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3vbwcvpai.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qduaxami.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tkadgvvo.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hgnfqxop.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qyuzzmsh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3imphgful.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dxclzkog.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mwronkpp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3txnfmara.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ewuhkdit.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3qowxxoel.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3bhshtfhm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3zeyasjcm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ljjpndjl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3wraffnvs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fmfybnre.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3aefdhsig.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ocqxvval.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3gkgiiwyl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rqwqdbbx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yfraetkv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lkwxnunb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iscqrghd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3bdleaqcu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3cbmddvkb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3mfwxmrdx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3rujrelkh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3upwlyovm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3xkzrysdi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iniubilp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3njnmzkvj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nijsaguw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3dnfujjtm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3pmykfmti.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ngwkxsff.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3gyrdvvfe.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3gehucmyz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3mqngkqop.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3uxjedoqa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3dviyvtph.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3lgeqhggb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rysfzcpz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ivxpajhr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vncosfqq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dqtxtgxc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ugmlqcew.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3gojuwldn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rivctmuc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dkkijwcw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zbdddhiu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rmhcdioa.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3eesuxjgy.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yhvduvcg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3yddzvvjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3odvyegzt.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3lihlbvam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hlcjlrkn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3eupxsvra.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3kiktoidv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uiczrsgr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qqeellpj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zankgnha.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ixsgewlx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3uncafeqf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3gpgmlhjj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mtuxzfqr.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zcauyatb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mqufvgcv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mclzdttg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3sjphkcxy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dxcysmcn.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3npucmcth.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3xptfitof.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3safwrhbt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fshmwmvk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cescefas.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ondxlwck.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hjecverp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zgetbwop.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3phmrexop.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cfmwbzpq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dxrjcass.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3pgdtdkea.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zsfikmwe.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3sseibonr.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wkrihfmw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3gtxdecwh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3snvzmyfz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3eyqzajqv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nfevukqn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3nbuwuayu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mtzfnynq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mvfitrir.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3xbktzokg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xsoyehlz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ezxqnysg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3npfsgezr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3qnjcrejl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bbbrkjpv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3mlaqidju.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3afkcoekf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3agtutzny.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3wjkrsphj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3irmfdlib.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ghatjygu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kkbwypls.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xuutxkjb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jpsxocvj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qaiyyvwd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hscrmqrp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ljoxswuj.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3imrkjtma.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3byllmbgc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bqpcnsuy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3eebcfqlf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3fynciyca.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3majixcjf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lrkxmdbs.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3yeapmvsp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3irwrkuen.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3skrnfbso.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3vubsixxf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3cjxnnwza.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kwrnajch.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3izhjhrst.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mmjtttec.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3egiborhy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vlrgknpw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zvathaew.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3fepclqbm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3nkvwvxxi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3tezvnuyd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yowbdtyf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ytunbffj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3enmbhewo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3kxjcxfbs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3rnwijpdd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hcwtdjsy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ctequruq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rvcetxdq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3mbgmkxee.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qtjxoquc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nflegcza.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3skjqjeyy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ydeabsrf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3iciphuzl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3dnddhhbk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mxmenunn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dhwmbxof.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hevswflk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qzzgctig.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ltmgdebg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3wutufnde.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bfuyflqr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fntvwgqb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hiffjocx.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qsqyqkbl.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dampojdl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3blxhdiio.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3aahbzykz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3snjqqjwa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3tpljxvbp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3gqjbnejv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tvnjctzb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3tknajbcp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3dnoejnsb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3tlfzthja.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3qbitsktf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ebrecaoy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3edhsaine.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezqjeskt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3kobthgpu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3xptmkjvs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3whdgbhcy.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3nnvyuiip.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3tyyfkuqx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ntdzuktk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3oxmymwxc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3kpyhojcd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3goepdqdd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3gvxqrefs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3zbdytvbu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dwmbpoep.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3rjaoubvu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3lrcmprtn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3akyfdomd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3frntaayw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3pxznyeea.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3nlemmimq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3gayhctdt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3htoxctgs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3lfjeduhf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3tuiidrje.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tbbsjhgb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3zmxausdr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lbmrfzjt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jwkmxyfl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hcceuita.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3rphwbksc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3lbayxxqj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3hezmjdgk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3hkvvzsmc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3iucsnrea.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ngwxbxfr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vabgkswl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fkmthsnr.html


<!-- 参考信息 -->