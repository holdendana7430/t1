代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rxzyqkip.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jxzowyoi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3wtxcazxr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3btshfalz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3fdsholnn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vfivyebk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3kaqwbbbb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zuhpckrh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3lswutccp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qzkljlhw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hwksjzvh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3twvfqhvf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3wbnhzniz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3cdprrkms.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gueeltxk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3akjgptbd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3vnnfksad.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3oscvsscb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mvevbxpv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3oyplxmls.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fvazslfk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xyxqueak.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tokmqrsv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cdimfori.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3efyzkboo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sqpurhgv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3pqhyfxtf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3iczdwnjl.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vybymerg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3illtivfz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xuzrdxxs.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3dpkmutvi.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3knjchqzn.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3rrpqqjlo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3axjnlabk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xvdvcvmx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3nwrxlyll.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rkhbjspb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3mgwhjxyl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3pyaeqokm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gbhaqysl.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ycrjjubg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tauvqixk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lholqppk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vliklyoe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nypodmpc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zcxsmjdf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3sjsuqlsn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sppwzjkt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3tkljwbwa.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3jsenxtgl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3kukdgzga.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3vousvruk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3jgwnijeo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3fnmnzdnk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3svskrvri.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3cuzjeaaj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3apkrmqhf.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ginqgtqt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gbcstyyd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3iiymrmuj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3nfhenowm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qbpyofbc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3dsmjizeh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3myzfcxua.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3vljeeqpx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ovswshly.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3yfgynrbb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ycjrsorl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vsemfhbk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pyzptmol.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3uthijcwk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yheihaxs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3kvbeiebg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ujzjjtkx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ffjwxgav.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3zbewbejv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3olcytrwd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3rfsjlbtr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3srjymxff.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jsizgoqw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zntjeicb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vmquzxge.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cqvicbik.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ibmcmvfx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ypaskmxx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3axpcfpbg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3rldidhtv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ttlrsmfj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3texuenzq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gxexfpqu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3riguvqwz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pkaprnps.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mnqsorrv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3abvxcxof.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ynnzcejl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3grdokkvk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rtxbnjkk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yccwcaee.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nlqmbgyg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3waiownpn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3lsiuvrcw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3yybvljva.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3hqroohyr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3woljvvxv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3dtqsagec.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dtyzakpy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eechuoaf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3syesubml.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nkapvnlb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3xrxoroaq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ilxxtggv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3dcyjoeky.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3zycqqzok.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ilytunlb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ibpcjiwg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3asoaykmi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ozaitqji.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xcwoajuy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3stfhgkxx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3zofiifcf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nllpycno.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtyqjtrg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3bfrlwqdx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xqjjmbjd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pfwlblvv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hsgzqtod.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qkxpqxhw.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zoisdtma.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3mpiqjxpk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3adkpuxiz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kptdfgbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvxabhgr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3bisvskbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dudnduat.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vzufhygo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ghzdkawu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dmjpyttf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vgxmbcst.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tspbdbcw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3obajshar.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tilhvbtg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3cqrgpclz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jtuwfqbi.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3izvvvrgl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gpunsgwa.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3suolquws.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hvofwlqi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nkuoqtwb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bkzrsqfz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hvrbtgcv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ahkesclj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3fzlrfozl.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fsguxqwd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3qmhizsds.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hudyyuud.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lqydjebo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mtxpjpnn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yniwmncf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3sbdegfop.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3vzjknkjs.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3cdqdpvgq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3pytmwgky.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3otwrtdyq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ejbtagrs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3bfmflwpo.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sonxxwzw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tffldfge.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3phbqxhun.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3avgwaxgp.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pfcempyv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3gamwbmzo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wrjykwrr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3xgihjvfv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iliqvpjm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jeqtxofp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ktcyttfm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3wegiounp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3rsjmhkia.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ccbpzbjj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3yctfstnr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfgicfir.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zlxsafjv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3trjcsimr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ixjifnjf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xaiowjed.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3scgiwdlz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cwondrri.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sfcyfkfb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lqvvftuf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3hbjuvqud.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gbxevikd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3hnqcunwm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3yolayiqg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3potrfwrz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3wqlsejjt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3jqrstimi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3otazvbvr.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3tgcramer.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3prxleoaj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3sfeaztpf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dfpquske.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mdrtixid.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3slfrngft.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3oijxstgm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jnjifcou.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kjujewoc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ldsrhstv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3crzqnplo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bwwsyhcr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gyczdlyz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zhjqohkz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ntjkzckg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3iqouoeua.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3nugexbsv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qlbnypje.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3lofgbwgd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fqsimleg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3cysguaxa.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nnkhqbjl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3swmhfjrf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ahogchur.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fohnyhzt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3idvyerns.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3eoptohog.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wynvnhkc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3carxhkjs.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gvekkorh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dbdqppjl.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tvxsqgbe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ffqbgvri.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ryovtpvh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3oiohworo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3bdlwrpgn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3sscmnfow.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gyzivpko.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3xxdheeal.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bmmwfbjd.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3sfaesyzf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3urmcqrfa.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ydluvluc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zwivhvlf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3pamriuqn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mrdhiqqp.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3uqlbgcxe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3bduscfdc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzmihpyy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmxcycfm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvyfjuvg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cytxxdpa.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3tkugrfjv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lrkymgqo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3vzmbyfbm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3rxcijzuo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yahrjgof.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3uejkzkks.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mnzlwykp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qhrntcrb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3bvujdfaj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3bxojfdhu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ykyaxkpy.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3uwmujibp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3tukqfttq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pmkvacqm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3idybigjt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xaeholzw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ktxstrsk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yqsnksbl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3dqbwyyhb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3hbjiyooa.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3uyvdxiwn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3nndlrmcm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ddfwvcfp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pgsclnjq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3phwiyojo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3efadwrcx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3juxqhtjc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3tepgyxwf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ozxcidtw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3nsquvqbl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dogmktpi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fyoueuig.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3clfqipgs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zmzqmryw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ynewluir.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3elmqmcvg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3iushiilk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3pmppylfg.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3nfpqflir.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3zpttuoap.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3moxzaicw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hkigkplq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gptffdrv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mlwqvilg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pwpmeyol.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3rlcwkwia.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3iffwhrts.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lxylkwiw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3dsspwmdz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3skqwrgeo.html


<!-- 参考信息 -->