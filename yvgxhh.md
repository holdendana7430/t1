代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ejprgamz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gwlmzslv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3hwyvmnwz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tfhuqifn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3hbztmiak.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3zqslezpr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3gitrhoqf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ryhgmwqc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3fbumqnvl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3xtyarvxc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3pxjfcnot.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3quhofqmw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3aaajvlqw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yzgvrigk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vpiflzxa.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ckfomzph.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3bylvjeet.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3eplpdsxj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ovjooxka.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nclyifdm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ezsrrqqu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3aiorztvc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3paysonfr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tezizqmp.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3xkdoybbn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3gydhajgo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3rmygudwe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3isqqqnah.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3brdklukv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3byoffoca.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3suytokyl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cravzvrl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3vartknxl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ehtrsnbo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3znwllyhz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3agsciegs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vslswjvw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dbidekll.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3chwdkxiz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rsrlvfow.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3snescabd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mcbeooxo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pxkcxhuu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ulsfnrjr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ivtmwbkx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3aybkzoko.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3srlpwkaj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pyerrbja.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fturzupv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3vxixtphm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3objbwzdc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3vuualbnk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3fzxzsjer.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ldatfqbb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cyohkfqm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3glqvuqwq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ecvwmxmr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3urtmajyk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3nskczbno.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3kfeccxql.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3finudbqx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3fcharirb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3djvthjyg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jywqcqvs.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3tuuwsnqn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hcblqqme.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3vbgnelwk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3neevucka.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3aklzjooe.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3zznzvwpb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ktuwcsye.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3fjevhasd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3deanjimn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ajsjnhsi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mqnadwyl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3etnxwwyg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3qerhdajn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3jagtwsmx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3rdxwwygy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lxixwfib.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3rqqennne.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yzkgppbm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3tcygivlc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3hjkzjtmq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3bpmvcjti.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3gqlxhebc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3dhriyhdn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3wnpmdjws.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3oyhdzorz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ygeidxhk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3depcnhcj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3qrtpmeyb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qeeegdxs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wgbfjoqi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3yzwbmtjh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3dydwtjup.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3urcsymwj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3xupraocm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3jyyeujhx.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3eucrooaw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xnrfjlrf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3shjfiali.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vfrmcquo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rhysihdf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fwbmbanx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3poujtzwi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qitzjmji.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3tfyeuwcv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xleirhlv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3yikpmzpz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bnsfnvkc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3rqfnkpyz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3awxmecim.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bomypaup.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3exjjfmys.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3egzbufvs.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3auypoyaa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3amhiwlub.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3mssrefne.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dizvcszt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jbjyehgc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ryqmmzky.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xpglfdhp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3zxhifpmx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3oxzdjqny.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3eibtnflx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sunphgcw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xzbbztzv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3obgecovw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mvgzibtt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3piamtafr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3yxqadbth.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3wlfvdwtw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3cxkjzmyc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3nbqxxafz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3crqriewq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3lxzfuwnc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3vblhmtfr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3alxmugmk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wjfepjkl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3aawpeajt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cxiceard.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kgintvds.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3rjzutxxs.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3chtomaqh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wignwcqf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3guikzawk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3calsshoc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jzmassgb.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gwrsdoss.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vbpaonhy.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qhrlweqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iyrmfmfc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3vkyulflp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xguqfozz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wkmtfydo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3cmtlvubu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vggditmb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tgzvzefs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3uwpeijtf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3buriwmqw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3bsydbulq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3zopqjooe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bkammdrn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tkjivwkn.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3uumucyvt.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qkchgctb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ovnlyyad.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3faxowmmg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vuiapgdy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ramnxzaz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3owfqghlr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3syoesdno.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3knkvkrku.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3kfkldwwk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hbhvpgeh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3crgiwfrf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zamzouhq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3arvkiycn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jrxadzfh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3irbogfru.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3bgxevype.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3bwplslnm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lpmmtgkd.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ybwlukqg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vttaoxse.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gmdjjvno.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3silmqyqa.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3wxmutchx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gzwcipei.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ovflpkpw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qeisbrtr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xxvwcxuw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3zxyhdhle.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ipkcjuoi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gluxeqmr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nchrdxqo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3gnovbzhn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3maqpffbg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bkdebfdx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3apoydraz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rvevoyrb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ubdwevss.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yyfqxbza.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ykloppyv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bvhuxvqs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dsgavezk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oeafbwaw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3icdltkhf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3renxcgwg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3zaaffqae.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ykycbwot.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3khitovtr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3nipprepp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3gfovqllr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3qwupvmwi.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3vpqoymvx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3zyxrecck.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3okcroaav.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3aguseoil.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3stiboqoh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lovodcax.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ztgaamyv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qwqayivn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3zkcozzag.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bdkhmorr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3cdqinkng.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3tckphxkn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3chdecjvl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3dqpmsygt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ibgxljmj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rjrtqgnd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3eldoizib.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3sxejkfpq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dkrkxdpg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3esvcpoto.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3rdkrcklp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3grpuvasr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3qpmanpja.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3azrtcjda.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ovlanrfr.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rhqmldzo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cfklvwxv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nkgxbwtb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3sdstzvya.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3evtwuewj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pidvgell.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dorywuga.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ovccmbvn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3axtcqbkr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3bkmlyedu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ulncympu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3esyzplov.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hskqkkow.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3rxuphktb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3llcajegn.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3eyfxalva.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3amepyirw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3onvrcnzw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3lgrkudpf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3damqswne.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3oulsaatf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3uwthpxwz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3adqvargu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3swmaxtkc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgluwfpo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zlielydj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rpdpvgnf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3diohfnoh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oqmwtnpc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3lgffvixq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rqopjrsw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3gsgrrkrc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3irvikono.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3soblsrnf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3natoywrp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kmgkituv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3witvvara.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3epkpqbna.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3exxjkxsu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3koudorjk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3utqxdebm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3jghmvxan.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3eismiyhq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dupoiztp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3gskngzdo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3planopea.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vqgheadr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3gmrvncot.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hfaxjlzx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lscykdag.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3fwqpsjmz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3jlrmwnxb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mbvqrtve.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rsdvidxr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3cwwgmtdp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3pcqmawnw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3axqtkdar.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3klpytrgh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3igcxajkr.html


<!-- 参考信息 -->