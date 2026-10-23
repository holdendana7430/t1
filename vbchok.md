代发 wailian999

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3bwmgunjz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3axkzpfmi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3zytvkxjq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3itzdjkro.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vvxsndlh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zcmastet.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3atpkzznq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3hunzwhnm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3gujvruby.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ukvljrcc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yuuobbqd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3osiaryfe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3vkkqvxjr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3wmuekkkx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3tdsxstoj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3vbgcxbds.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3wkvxhfrh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3yuwikzfj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mkdersui.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3awjbvgao.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fllkkwjh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3eqachqby.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3wifvjtkq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3grlxywfc.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ebpzkmgz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3cuhutndo.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ffwvaqhm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kmzriugf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3elcjnbmg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3otpsnenx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ffoczwkw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zmijupdx.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3kmdvayun.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ihwjrbcw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ofcsqxpc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3qdurdhwy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rpuaduge.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mapmecpu.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pdezrwil.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kbuhpmcb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3vyxabtfw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3snbyhuvi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mouiubdn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zxqddnqj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3oqauclta.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fhggwzyk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tsynbbrm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cwcojjbr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xqazprzh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3krhcplvh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fttnerkg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3daknugfn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3uvyehjzt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hyyktdhr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3rxcdhspl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cazhprzw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vocrwrvo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3gcmshqdx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ravzsctq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3eueugnqy.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lmzighuv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3rdtagegl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3irefothv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hsmjmjmn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wxrwghen.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xuxvpvov.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3zuevtstl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3wzangwhp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3xkljugib.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3marmaerc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3aswouoyh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3inmoqogz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vehwhoms.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3hitnukvf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3szujrxwq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3psmwjxct.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lhwxljsh.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3mdtvgosp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3klcsrrcr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3gjmxjjod.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3djcyaqtd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3bupwxcsp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3tnqrladk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3zyipbzjg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xndgkhkb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3xxjighzx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3pdyfwuwh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ebxpekhu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3rmdozwpc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jlrtchqc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3kvmmmmat.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3lavkdizg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jztnhcod.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3lznghlls.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3zcuzrpys.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3xlicdbfk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3amhijfjo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3txitssmr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nhqiglla.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3dtecjtef.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lpbqatoa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cpbykfwg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ztadxcll.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3qqcpabqs.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3owudlwje.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3bubevckv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3zilioggq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3wubmysfu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jiskyhlk.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jlccutcm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lchgsqow.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3srwgeklo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rfevlwcy.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3iikddyij.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uxuxwlek.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3haonjofe.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3vzdcfhpc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3osszzyks.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mxvbjsmt.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3clbheohx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3msejynxm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mfpjfoxn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ixhznfim.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3znsnwozx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3sqbbxvga.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xsnixfiq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3tndwutqt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pkkqcdfj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3djyagykx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ronquynl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3njxzhbmp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3vqwkqgxx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3zsbiatzg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ktmxlzef.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3prkepsbd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eiuvmuwz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rdqqktvu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zclbtfcs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3yjjurmkr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3sxizusou.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ewptxgqx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3qiinpkkh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3meqgrjak.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3qhfxwalc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3aaghnwnf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ibydhstr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3fahtgexg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iprsdaxq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3paesizmg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kjhfmagy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ozyepmoj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nfvomwaq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3azjuvmrq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pengoukx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cotamjxd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3aaeluiia.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mhiivbtn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ckdfmmwk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3roloxgki.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nwcnarid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cmijibfc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ejqlysxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plbytkmj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pzowodik.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3zuhymgzl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3lqkbdvzx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jgmfajrp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wkxaazju.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3kipgkkwq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jajsduch.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3wlrcwrwi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uvqskisk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3jtuwwisd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3eutipwis.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3benqjxha.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jdbiycyz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ubgwdlti.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cyjcnikd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3nxmxjxtc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fpwgmiwy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3drxjrbaw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3drfxdssn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3jptzsawm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ytqgnzhw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3frkypnth.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hdnadsnb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rxoneyru.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qwbrgqba.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ulizxard.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3cwqltnsq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3lcfviibm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vsjkdfka.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3omauysjc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3fvdtujlq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ewlfgbrd.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uxmdxsfq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3zqvthdza.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3yvoiewwn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3peorxduw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3mddpwnde.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xghqghqb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3wysvgfbx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ldywgtyd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cyewlale.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dbvddlag.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vxkznnak.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3qorkfqgw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3busznnvv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3metrqjzf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xglitmsr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jnufdsdo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ekotzboq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3opjcsjib.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fccsuqno.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pgycnvyz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mmcnvjqc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wbxybqkp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3guzcatqe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3cdrnfchz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dnhqfwyg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hcewzyro.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hshncuab.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3gruaqzur.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3olozwpys.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3tquobncb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3wuknefom.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3yxvzxdgx.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3kqflcfxf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3zgnbhcjy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zyvbunnv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3relkcugp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3itwwcdmd.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3dhgkjwwq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vsbolros.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dqxtaiji.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3chcuktyb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3cvheyljs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3zqbwantb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ctcryzft.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rrhctatg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fpulwsfi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3srnmfgqf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wzixywes.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bwodtzyl.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3paasfkpf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sqqombtf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ftvazztk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vyhvymhz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3itdbtcig.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3blbhotrp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yshbvenj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jmclubvj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3hdylyyhr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3bbdvvzsh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lnbbftdx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ylabuwfj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hanqfwfh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yxbxyvpv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gfzqemic.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ruvpdxmn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gfvrwmnp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3uoyndjvm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xaedmvsl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3fzevvntn.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3qmgztdrq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tpaxynxy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wkazmutp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3pegzegzh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3szqzvmhe.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3glkaiwdx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3nvskrdzo.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rifulfpd.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3jreldvxt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbpclmtv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzxgeohv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbslsxkm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3blickyav.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3nmrjvxhe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ksqxxiiu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujovzghh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3gyfrezpe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3hpvepinq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jolmeouh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3wftppubh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3qnazgnoq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tqnfjrgn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3zmqrnhxx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3isjnjeqk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vdizeajb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3nyyufprv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kkpntqlt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ogvhlths.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3nqudegnl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3xazhtmas.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3cvkhrvfj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ohrmudup.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3fkgzjwae.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wnhtsraw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3omoivase.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lsgjiahk.html


<!-- 参考信息 -->