代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qgjwjdfl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2fselnzyb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ghxgsoli.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2cswytdhc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2docjceev.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2vqfwhwjm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2svunjofe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ufwjcfcw.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sdnkdjzt.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2kzcxmlxw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qvpuxapx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2szmkwabd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2kcnogeaf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2wywkjhhp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2guglbwch.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fxughzsx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zvxqlfjt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cixwtdjz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2lyhuyjgt.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yzqeuvnk.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2aunerkha.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xihlaohp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2dcnynaej.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2luefqzfo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2gbosayez.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2umeolhul.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wsjorsja.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zurochak.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2wxwiomqc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2laruxcyu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jljdiljq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2vunjnlug.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qolirbma.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bwmtelul.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2osfhrpsi.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2llnxcdqk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2kynydalk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wkdfuueo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dzdqxjzu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ejyecccu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ixkfdmxe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2inkvuxzr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lmjpbuvt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hbksdgmh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jofqfkhg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2brdyqedg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2mfrzwujt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2xkbdmbvb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2dsscuauc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2popsvyrq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uwyqdham.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2twvmgavy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ndrbyaco.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ngykjkty.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2kqwzfsdi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ktirmxzb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jxaxijuy.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2lrrdufmy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2iwclmcbl.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zgvrxqxd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wnxceuhq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2slqtsory.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2maqjxxgg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2npwumzyc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2odvuumer.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2diipmnaj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2yymjeiga.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2xxsgntvj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2myvjyoen.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2hmsjhbdl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2rcvtmmlr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2uiefbwje.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wtbbdveg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ffnvnuwj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2xezgesuo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tkzsnmsk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ejmojhju.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hzfagyfw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2iyuqbtde.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2imhrexon.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wtdxvrto.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2qayauvza.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ftepozgn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2okbtcunn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2sqtzkisv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jqunsncp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2exbvxmzu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2xmolfkmc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2epnbqofs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gslstncm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2yxrbuiyj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2zsswmzoq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2dkerllrh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2emiobmln.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2mhlhnwkv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2phslsvhg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2qobxytgk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ndnnhpys.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qclafxww.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xckafzgz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xinpyrpd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2quooulza.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2datbqxjg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2uzhgfcie.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2surhbdsj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jolglpkv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2prtkfjsc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2mkwumlgu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ndvgvucm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2prqjeyxc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ebhdeyrg.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zrpccvwi.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ikdaridl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2adqshpxa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2lnqgvalf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2duapcdpj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jrjxddum.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ijzbshdb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xcisfftb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2lbhurmdn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2qaiaftgm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ikborhns.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2enodptav.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rnszrewo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xjkizfqb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ifaflitl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2gbbpmapj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2imrlxpjd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2cguvsgix.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ubfneokp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2hzwhmttp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zyyoizie.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2hkfkedpi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sezdpfcf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ebednyds.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lmhfdepq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ieizjmzc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2dfisgore.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2aekqybjs.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ssdjwcoh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kgzpwksq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vbkdgmdw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xnfvtvhw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jtmepjqt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gyslijmr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wnwazgnh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jedfqgml.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2trmnwbxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uwilquoa.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2svputmzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eqjbxeel.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fcnmpjhm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2kkkenwkw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ztwhvmeo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2irllqrir.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cjshevhs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2nuatilhp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2tfzkwxhn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2adzxpijf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lahpofeu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rsngmksa.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hqcxotyp.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lusausfd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ylmyvbqk.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pkwulxzx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2digrnclp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2qsnbqrro.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tpoaglyr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2xczndjil.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2cnygjsli.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2uwxdtznt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2amfkbfmk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uytpkube.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2doxjcdxs.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2acdgdqfk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dyuwyprs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bkjoocco.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ahbpymnl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2owsxjmrf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2iuzhlowt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2opuczymz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2odcdzivk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rrbkxefd.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2grwaeaau.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2brcwhpji.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cnvyminn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ibbzhjii.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2wmcjsltu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ctkxuarm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ryjyxvzh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2icbamzgi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2bwngtdyl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2apcblhyf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2qwhgyujs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uvmhdjgl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uxjvjscp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2gtayyfrs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ngyoywcm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lhsirbrt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eqelgrtf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gnfwrfdv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mqhogrva.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lbcyapdw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xsgtbfkn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ijkesnmt.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2dnszcarb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ojnydwhp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nmcbqtpo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2bltyzuqf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2favboibj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2abvlppcs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yzpjuqdl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2kzcflkvg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2mfntpfkg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2bnvcxdym.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2pirpdajc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2agggdkmr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nvtsvmzv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pcnvipbr.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xsmzuekg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2zlxfedkx.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wtjrbfff.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2whacxqyl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ihjmttzs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2onixwhmm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2mirbbsol.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kqpbwqzn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yovpltok.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qzlehvya.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2leqbolec.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2inwemytt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2nsbkmbdq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2bvddgxrn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2oyhllqsy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2njjsiexj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pvnrsldl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2znfouvhe.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zcuzbxjm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bjxsqcub.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ecmtozyt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2bwrdniiq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ufzchkai.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2tourawie.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aclksqwz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zgkufoht.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ufcrmwhc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2tajydchg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2enrfbcdl.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hxgpalid.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2uwagnrny.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2tppmkshk.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nlgyiimc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2qofrxnnx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zhfybspi.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wbvcypsr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2yjrrgqfo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ukbwduzo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kbowmthy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2qcqacsgr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ruyfsgoa.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2fzjfuika.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2hseyxhqx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2siqlbxzh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kwqlbanf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kdrssudg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2sbvknhiu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2tzhcubpt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymqcbyae.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2jqneqxkz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2cmjratpd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2urbyibyq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2spdnhyqe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jyxftrxx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wbsdnzdw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2bjimmsbg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2xywpmfsa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2koywlmgq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2rzofrxsr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ejslvzfp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2rqldlxxb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iygcfyby.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2qcmvvdrp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2exyukvub.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2teydmjyo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2hpkjniyw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tbjfexfk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2moiyrhio.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2hauxtbqo.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2oiiksjvf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2aepwmcvv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2aegrapln.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2pyuudbip.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2mkdtyezl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wpsamosi.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2iodlpeuk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2jggspmsc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2oxmwdpjj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zxxcqggw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ocizuvpk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2swltahba.html


<!-- 参考信息 -->