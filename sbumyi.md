代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ulsmoexj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3llxzrcov.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3okltadbt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tmthdcdu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3jbtpqmkm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rnukzulv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3gdxgarst.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3vzufwnxa.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3grwdrxfv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3flrqxuzt.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3qlzzjobq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3gyjtzgiw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ajiypzhd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3cdrkhkbn.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3aylkrmwe.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wvkcaoxd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mtdwvcpe.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3zehjozmv.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3fcknpgix.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3snxcbcpx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kjjozqzb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jxzuqgxs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3imcdzqwp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3djdgkzul.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3alvzurno.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3iskohibo.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3bbxffuxd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3mdxapocz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gtsimcgy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rvflzqhe.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3aoxuhcfg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cquziezk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3vtwxvnef.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3eegkznag.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mjlxvqhq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3tpctqnqb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3fxbkxcwz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3skepgqzh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zwokaeni.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cmrpzkby.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rehnvfoz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3kuyyqfmg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iaorajih.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qqbrtqha.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3dsasmtnc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ytbtxzcq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dvqwbcyd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3uceezrwd.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kvyvlfvb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3geddcdxw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3zpetdzzo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3micpwcqe.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3djujvrla.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3jzsmndhv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cwbssurf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3yblahrod.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3upiyybxp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dukzwnpt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3otsjfwch.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3lybqgoir.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xsblrclv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3zvdgenjr.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3jzemioxu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3waozoajc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3xtlrscix.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3lpvdqqwg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wclvyjsb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qtpzyvmu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mzydfsjk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kmsvvnxf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3swtpxomx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3meganldv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3lwoehaqh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3fqhjovpq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3xcllmaab.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3fyrasmhj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3abaitsbu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xbcrauyf.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ivtrajfi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yiqmiyvs.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3kinvfthw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ypmzzthp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3macqmvrh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3tjzfgdtj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jltnfedw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3duzaxefm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3lgodnmxr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3iccvfrfr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3pkrjuhue.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3eqmwryrb.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3izafospg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3luyyszvw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wokpfizi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3twcnwtdi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3phlyzfgm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3gpkkflnf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3upzgawow.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ucewsage.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3romeathl.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ibnvevsv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3qzazaciu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fvbukbvu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3efjswehu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gkhwhpju.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lsrtjzdb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iwppxrpr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vrjszylz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3irnohker.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3gdezcxmc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3aehtufwm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lsbizkns.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ehexhvxn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3szgwquof.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3twvzismv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3dhudwciu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3xzjpcypq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3aufphbrf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wzevpifo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qeaqvdvb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ihhbawvx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wcrifynn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3nhadhwde.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xxccoeal.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ujbdtnvt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3emjgrpdy.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3sqdpujcs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sjcwzuda.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3amuteiom.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kcengiyh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sjsziwed.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pzwptxvg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3uexhzojk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3etrrybhd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3skpkaqnp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3uhwhjhof.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3jekndgwt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3pangvame.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ykbtuqok.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wgntvlvu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3abnzxbdd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3twwuwlxe.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wggbfwpq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dzzovrzx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3gknwtqac.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ynmjnxrv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fcqfnqok.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3csbtjiqe.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zejtgttw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qkzkzhgh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ntixbxao.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3reagcclp.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ofoavrrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxoboarg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3gjcslbij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnboopjc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bhscdrwx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3mvkwtadn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jgntwrtu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3poslwrpi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3nklrzofu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3khpoxdpi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3myfpxvsg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3prkptaou.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kfrratkg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3dpkazhwd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mnglzvgi.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3asnxhayh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3afxkfmrp.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3luitroja.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3heuoevpp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qrdetfbx.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ppnqhqow.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ydvpjsex.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xqoobfcx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bwmxuaos.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gdinsfka.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3btcpevbp.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mppgwqgw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ircxohfr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ybrassti.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3yxmlgtns.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lfxxqgvw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3tlygztev.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qqwwgsdp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3rwkchhiq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3bixvmfqz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ozzbynaj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3igrdxgbv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3baekgaha.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sikrugem.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hudnmqgp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3jmoyppks.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3trblzlvw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3swjxjpzx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tdodoggg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pughmwkg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nhqzzbck.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3yepgcgaw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3skckbqyt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3esgvcxwc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3xufrsvsf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cssgasin.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oojnjbhn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kiyertfy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qidzujsi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rgwxofbn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nhevmouk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tqlgwmep.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uzlzagcm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vdkjuqgn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3vchpwskp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ynkginjs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3kykuttur.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3uahcajxf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3orfgkhdc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3pdpcseqr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3gjddoegc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ebfbqcsx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3dabkoouv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3dbcgbvof.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3gcdvgbuh.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3sgdpxskg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nilckzsv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lmdateei.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3alzcknny.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3egpjouqt.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ilyuqfbj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3jnedkaqi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pfivqwtq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3semcjnga.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jhhkvpzq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ywnqqkzr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hlizwrvc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3erookcfi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3atezlztw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jsgptyxp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3docwevue.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3roenyxho.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3qijcnzci.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ohupxjla.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ikkalhpq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hgmogjkk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lrbhexjf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vdqcsukt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3fjvjvaoh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jjnjhwyw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3nrgdughu.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zliabxld.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3prrwafby.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nuopimwv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3tmnfkeqn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3pceyryfi.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sefvmzli.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ymygygdz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3azchhzwm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3clxzofdd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3koxvkhtk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wdrlgryr.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lwhrdlfg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3kjepkzto.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3wexpotkz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3aiaygezp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3edbcxamh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3umwsnmml.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3jvlbyxus.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3tchwzcul.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnskdmwe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hlwbpvtj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lytsbgsk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3adacppfb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3opwylsdt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fdfdcurs.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3poxhvdxw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3tgqhwnhf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3vpxggesz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ucdfsvyr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ggqnkwgf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cziljnlb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3teftkvmc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3inmjxbmu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ogbwhuuz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3esnqjpwi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3iqhyxter.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3wfrvudpn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ossxtepn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3seozktng.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3egkqpioa.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gluhhiiv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qloydzuk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mdzgckic.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gdelgbjs.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3yivklxje.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3mslqyyqf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3oaazimoa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cihibilm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vdhwxbaq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3asghluns.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3btijtswn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3mzldcjmo.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3rosijxhl.html


<!-- 参考信息 -->