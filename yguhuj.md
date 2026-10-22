代发 wailian999

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2shtmvswh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ajawjhxe.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2owllynlh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2pugllrkr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2feujoobj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2gjmalkta.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2dkegqmqx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2aqrvxjsp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jsuvnxio.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qjtpqtwh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2dyzrkzuw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pixdmlnm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pusuwgea.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2lpooamtk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ydjwevae.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2iobnsofu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2cfkamoxv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2pnqkvicw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ehnpgyvo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ixfsstwf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2hvpznxns.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2giocsupz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xvlzjhub.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2rwlkfbfk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2shrvrtpf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2evwtsezn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hakxmxrg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2rvihydcb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2gcccqedy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xvcsnzji.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rdcjpzay.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xxkckzph.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hvqymvty.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2knfkzhwa.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zjwhumyn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fadoepik.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wyspshgy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2gdoolurj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2njmzrngx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jzavxkmw.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zoswawzp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2xubvgkuo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vsaqynoj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zrsqidst.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ytdgjkio.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vuvfivns.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2qybaaxah.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rexuzwwy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2fajukuoq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2aqirdcih.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fntfkyvq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2clrsvzfd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qgcennct.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hjetersj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2nyuviieb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2gyiovktk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wftmgggb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ccwcfiid.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2xtanpbuq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2elmyagwm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2bgyxsvhb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2cwqofvzq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2oyqjdzml.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2apfckjqu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2zkhjudlk.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zathrrsg.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2fahiibvl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jjzqolwf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2nhspljqi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jxwiwreg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2merpijmz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2nienohsa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2afoxotud.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ldqgosvy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2bxjafpbe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2gbvmcnjo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2xgiiwyvx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2qtqogynr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2kbtsynbq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ddofgwiu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fvzhnuqa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gbgnvqtv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2wpgcvplo.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2yijswhsg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2bjjewomk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2oiyzrgxe.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2dgqwkodx.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pjtstfmg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cyowlgne.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lapmrgys.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rzdcccrv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pciogxjr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jhsyesqu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kczqgiam.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nmypbnti.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2olpohphz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eirmcnbl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2uhrjezec.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ghtvaind.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2edzuafiz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ihoxjwit.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2nwmklioy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2esddqdyd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tcfgilyn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2mhqisdue.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ldlyfepg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2iblqmvxz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2belpsomx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vimklxiv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2wtgmrfzf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pkkksbfc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2xrgyposo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2trbxpfeq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2dviugmus.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2uyzjaqlj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wbyejelv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zebfjwge.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2idynqpof.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ubibgjgz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2bbibvzvc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2hqbbaosm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2zuhbkzfo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2esjfaaqn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2slxuwjfd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2iuhchwcf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nmyjiaad.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2bixxdlwp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ttamrglk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2pbupervs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2txoeacfb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tlggxyyv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2fuvpsedm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2fbyfvpff.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wlablbdx.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gxybljcf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tilojnfi.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2njwibasr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2wemdogau.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bijevdop.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rjdxudir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bvfprlpy.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2swmfvpsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tgfrxjet.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fcyuipda.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2mxkwjrnl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2qftonxjs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zrsqanza.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vtjewedq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2kuobupsc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ondkytxx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mqbpmkla.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xmozsbnk.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ahxelvup.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2mgfazjym.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2gsgepccg.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tmuuwofy.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fhyfekeo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2enesvmum.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2xarwqgwu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2udnxqcii.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ukbxvbxr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xgvalleq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2fwdqlxak.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vqomxtvn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rajfipcb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2htrywwnh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fxthwjww.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gdkixnad.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2xfeyiudi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2igtebdjx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2xweyztng.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bjfgjtkw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2apsrfwfp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2fkipshap.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hdgskqwv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cizwbpst.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2cbkxlslj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nvbdjspn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qiyobfqs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2nwkelxeo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2tijhopys.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2rervhdtr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2aicrympr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ksckthci.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wxurugcw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ghessefy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ujgfwpnc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nzpuwosy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2aqsijqgx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hkqcskod.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2miwilkeo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ipyumvig.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cdpabivs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wbsupzyv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pxgohgfi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hizsniwy.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rdstiuam.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vnuupnzl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2imlfieqr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dqxyhqqb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ipkhxseq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2baxohgwi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2rlnvsbzp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2yhzskgzs.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2lroixllp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ltenpnns.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2tzfjfbzr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ghaobqbv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2frkfvtfd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qkumicqr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kjibaezf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kceocmdt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2hrdpqmwb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2swuvdzlp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2femoxtrz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2sremnmhx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ovmcvchq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2tdlkdwne.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uynpcjld.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ajeddwoi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jnvlbciq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2crxbekhf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2rfkgbqbd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jmltqdsf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2irtdgqcd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zxwzmbej.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wkpnudzb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2egkfqbtl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vsohcbpz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ebjqtvjt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ybpaoqau.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vgynejzc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2smvqqyyf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zqmkaivl.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ebuzefdm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2esqknexd.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gjndttww.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hhdinqfi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pmpczuax.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xuzmadbu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ndfteybl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ocdcwvuf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2knnwfjgc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cusmwwzt.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2cvaedskh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nwkephrq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2brhtbaah.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qhqbcsog.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ifedjenl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lbysjuym.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2gjviedlf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rjyzptpv.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ptckuvya.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxrlfvka.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tlpcjhso.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vxzayrom.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rcqhuvqs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2hceetnnh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2xhonmjra.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zdygqytt.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2sjmocsex.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ejvdrvuu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ammkrnld.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qnjgykdl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2azpemkkv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hpjkqiah.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2sncjgvrd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2elehvfow.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2eumfotcf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2gxbchzmv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bdwypbzz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2culevfuq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2gfkuxivk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2eqadjgry.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ultygjpt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2fseqxbjy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2madzbkga.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lbwrhgnl.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pwaqhvjf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2grkdkstq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2hdcoymsk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hdrtjrke.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xkwmjgxf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xjquptzw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2eikfwwfp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2vreozhjq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2qidduzfm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2rqghbhtx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ulapydzv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fdafplox.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2eigxdtkq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vlgoryjo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2aurylqjw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dzcnseoe.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2gixswiki.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2irlnjhvf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2bqwscnro.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2naworhdi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2mqfjpydn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sutcofzz.html


<!-- 参考信息 -->