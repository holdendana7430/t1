代发 wailian999

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xeydqjoc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ccldgqdb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lbtwsxlg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ssfmtgpb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2igeabakc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2djzmvacm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2anhdkzym.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ibcvpaet.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vrkkuisl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2psxjesuv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2eqtogute.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oucoeymz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2glpvxofo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2gskaqgkp.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2fobgwwpm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2orhbjmvx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wjsgfevv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wofrexfr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tkboenwi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sysndeiy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2zdqnnqdh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2lnopsbok.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2akxxkbdn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2efnejmpa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2clvezbqn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jlmjlfkg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2nrxzuouk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kegatagh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zlxokrrm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zrzwppxw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cpqjjehe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ntoyyxpn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2gbwddlyz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2losimegx.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2hgjijocf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vuavgzgy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2udeerqdu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ntfhqwlf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2knegabyx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2jqkwcgir.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2swxawlfq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2lnoasuhu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xxbxlfcq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wfsjfpec.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iplkfwbl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2tnuycjer.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ougsyadv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2bbfqgdpq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2dhwasuje.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ouldxqvx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2opaqnicw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hgridifh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2bqyxchgi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wdegqaqx.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gvhophbk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mnpiooks.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xpfnvccy.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2oqrpwopx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2yizroomz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2pwuzopgc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2omrkfdbn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2rjhszmvm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mjxjcjbq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2gxaeiemh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aoiswljb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2lfanueyp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2hehqpdme.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2smpkevcx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2qacxccgg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2dzlfterp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2pkmusdlh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2wrtptmqw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fwkqjpey.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2vypvcakh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2xzeavubf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2kjoojipm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ifunbjhi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ikyhmwft.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ozdvmoew.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pwzvzooo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nxggdqzk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yponatos.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2sgtnwzok.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2wxqdjlys.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2yxsvdxpv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2zfgtilit.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2hyzcuifk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ystumopw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ysruzmlj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ipdurknn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wjdneazy.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ttipnyji.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wglhpepd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ebipqoqy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oyhuyhcm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2lzahmveo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2xlzwssxu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2xljevgml.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2zcwtngrg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2okmixxau.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2aquaomnl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2raxkfgag.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2udjdrcxp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ejikcmhz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2dqtfrwta.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rssxowwc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cedkqdak.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ookenxbw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bdlwzdsf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2fqnpfefz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vwievgia.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2izqbyzrk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2kkjnsxns.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2qlynzave.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2hmmvsqtp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kdtbabby.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pxjslcod.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jrkvbsrg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2pikqsejp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2jstwdoaf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jglrfnyq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2laddhapo.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2kjppnlsy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2efvdkalh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2apxvzdsy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jlziwkjl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2gajlfbwu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gldsnpvz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2yzfehwah.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2dujpsbyz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2yvtbzygo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2phjloqws.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2fbngdutw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uznouopc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nyhusbiv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2badieeuu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2eqtnxmzu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2sxcztkqp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2secwgkyt.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vfaffvwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwhmlytr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2jchxxpdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnpjnwgf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wrqkcqef.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2uehjoyny.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hwmhswfw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2anlwkqmh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gkzuaznm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ezosqmzr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2pbcefist.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xfbewkqs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bizzehvm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ovbmmaiy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hxvmakyk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cgnslgxr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lodujiml.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cutdeysi.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yninykrn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xiacjpdu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2enbmgins.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2xfmsmtvf.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zxrtncir.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2uisdbeeb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dlbsfebn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ynsohmfl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2naonpkxp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nuptjydz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2euccktcp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2qdrlzffx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kfhrbzds.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2psowohjf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sdxhdyvi.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2eujbuskh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2lafvswjh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2enmvuqtw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ateilaze.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2xnyvtzoa.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hbqxrcvk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nqdcsiqn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2dzvmjbjj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kaxvmekt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jqjszmqt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pgichfwr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2qrfcryyb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vkbjnrah.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2hrgwrqrr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ievvshnt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rzmawdap.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2rjauogho.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jcypscky.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2blnyuvru.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hfxqgghq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2idfcjayx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2otxdnthl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hibeldoq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uhgolrml.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ruzdqygf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ndvexrzs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2kkfurwzo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2aeiywxet.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wtikgzww.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2knxuwtrp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2rvahwgjl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rnmqjaaa.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2mdejqhgh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2tevkbdbt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ojynyxpi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2mpoghwrh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2zzcytnob.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ocwdgsrc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hkpcxreu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hsqadmyp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2gqmdklia.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2oofsrrtj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2nycqugwb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2jgtseatt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2rvyrniou.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2yzqofpcz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mgdlgucg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rirmpusz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jhgzmzwm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2swffrqjy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cbhxwcky.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kmrgrbnc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2arjkhvao.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fvunhuqj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2hgztumkj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dngmlscq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qrosruqr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2umzymgci.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fvfgxmqu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ildhrakg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2vlxlvzuk.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ictmpnhb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2scsbxfac.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ntcmsmnx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kmspwfpo.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mqlfrvnj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2vpxhkinl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qfurumnq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cflgjncm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2zokylwzr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2uhgxxaib.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tqloffsm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ensnejqh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zwsxllug.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vnipkzil.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2aumoseqe.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2fiuwtfgt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zjuknafo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2fxxtxhhc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2etlsychv.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2vwcrluvt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyxzjugx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdujrhjy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gnttrdui.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ldvvokas.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2pxfzsedo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2igjpojep.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwhjmpyt.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2akaommuy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2jycdwqtq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2csorssik.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2awabhipx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ydgxypyj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2aperbcmd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2sfetatus.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2idybfmho.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fidluogu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2dciiigcj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ducchiwj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rmoprvnr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gqjpkrxb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ggvitwxk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2xoezagfw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qkclhmmf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2nzvsslui.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2jwnyenaj.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hwasfodt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kelgwvpb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2lxqarbix.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gsxznzqx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2keiigvvr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zyszdgmu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2wzasteyl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2nyhpykpl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2gdmqhkeb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2tkpejoda.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ndpegpsv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iqjmuxyc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2isyzewwm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bstbhdnm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pyklvvsb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2mmpykwdh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2yfrpiusq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2uwrytsvt.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2rbuejyhr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2hheufpzv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2khowsrsq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2svzektld.html


<!-- 参考信息 -->