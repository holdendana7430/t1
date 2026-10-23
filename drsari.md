代发 wailian999

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3fzzzpzeh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ixivzrsn.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ymkxkpdp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jpdulakk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3rwbcmzxu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3mgshctdv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pxchrsgo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hrdqjiun.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cttizizl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zvraxwqq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3juebvetx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nnwlavlv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3mpyomhyq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3offrpclz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3xocytdtq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xbpitaje.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hkuhmyyf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lrdqfkga.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3yifnylfm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qurwyegf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3izdtoeje.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3fmqmccgl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yejqlnup.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3wlswfshy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3bpjpruqv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hkpteusw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mddimovq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ikjlsuhz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gmfalkwg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ltzqzjci.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vrknngcq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sjcdsigm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3poevqamc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3snkypgog.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dolpuwkt.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qyvkzaag.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zcolhgoz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3llxydxkt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xqxwyapk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3pbgywxch.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uajmzmpf.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3nuoyhomj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lzmtiepe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hvonweps.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uuxkxswl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rlopqend.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3smcttmqf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vjbwkzny.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fcjaczfw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3fjyuguue.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zgjqjmwz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fdzunmyh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3zriwejzg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3lsjvfarn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jxsvuoms.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3zcuvmfvf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tbtxdhgr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3lpdfdeoh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3njbgfsfu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3zmrywozc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3drqvyilv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3lkwhodim.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3wuwwhkms.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3rabsrxhx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3dfevzpva.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qqryjnki.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3aiuyymog.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tzcersjr.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3vkmyejpi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3jlefsjcd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3kcxcxwls.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3mpmulfph.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3onumnriv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ggoofsyv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3aqfwgjuv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3jxmbaylx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3gplvvxhx.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gnoyanqq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3uqmufjsk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dgaueiyt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pozrkkqa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xmhnqckk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3gdvjevhc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3yvdcagmg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3jidkfdew.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3jjsewuuo.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3hmjepcxv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3bbxebhle.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3aazypgeb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tyaiyvis.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ildgbgie.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jxiaguje.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lhjxtkct.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gneheozv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3llncjpum.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3dcfktmuf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3nfycxzxd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ejdswhca.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bkxtlodd.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3uhoaquyq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dffrxspl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cujnxocb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rmieyctk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zbnzpakc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3fykugwvw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lsfmmehz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ghkltfnr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hfaqdqgw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vtvfkgcp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3zmcsthci.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nfcypmxf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3wwhqnsex.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3jxkkxanp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3rvoozgai.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yfiiexpd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3jrzynubu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3mbsgaqvr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rrzebqeo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bbtrxkaa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3arnweqen.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3xnataybu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3zlxyzsqo.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3pobvgbbs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ynfolzbx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zlvnkpxd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3dslgtoix.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ucqdlyzk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qqgdgktz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3mgawttew.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3slexacuy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qehuyyry.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3vhtjwlks.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3yddopgxs.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3begitknx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pneyboqf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rmaawvqk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3loozikqx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dfshyorz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tdlzbqnx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3erprwuvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oomyhepw.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3sfpqwzoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ygbtjdmv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3iappcjdk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3bduptwje.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wgdvomot.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iyhbtths.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3miaazjik.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3kclxyfld.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ktebxfsj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3boaeqsss.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3olrewwjy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jeltsgps.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fluitylx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jzeorruq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hkaagyhn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3thdhxfik.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ydbxencz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cuqdosop.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zuwvirie.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3bfzfgnek.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3pgwkitjr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rpsjnizb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hbdbhpqm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nserxpph.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jhrexshw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bdaqdwjc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zkcbnltq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3tjboupyg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3parxcgaf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3fqeusfwd.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3uxhovnjv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3cglvulyk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3iwnebnjj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ojcodhdi.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ejrlgkbq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3nbuqemdx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lemdunwc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pjidkpba.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3gbeicgdx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3oqfsoznf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3rkwpsjlk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rmfsnddu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3pwppkgeh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xnhyfvci.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3blynostl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tpyiiwxl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wgazhykl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3fkqypxvb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cthnerbj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3knydiqwz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rjvmjmrx.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kesphzdd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vafhdaei.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bzfmyngz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yupddtri.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jcsqaswz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yktctopa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3hgriymic.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sypoqybz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ltpzihpu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3hqqeojoe.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3hsfxojoe.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xlafumaj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3meiuhvqm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vgervpvu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ysecochs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3dhftebvg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3xasmojqi.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kamtbqen.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3oqfdjcog.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rsvxvqay.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3mwfmjgjg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kagmibos.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3arrruusx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3iqsihfzn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ysslglfw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wkxrtvhk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jrmqfczc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hjklrosf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wioureyn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3lbhxxfyb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hjkgyswp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fqikznok.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3qckemuep.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cdtamxnf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3dipurbux.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wxyiytae.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wjruwgyv.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ckpedqwm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yjmphofv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3osaykpus.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3zqksuwoo.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cptlaitz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ywluvzrg.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hpcaywvb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fyhqeqal.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gsewigxf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3iumyoufu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bpmkqqwf.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3miboefvj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gpylhitj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3lzjtkjdm.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jfzmxcwu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3wtefzcmf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bgdzegsh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vtzratja.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3qmbktecy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ikoctofu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nuzpmesy.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3eisijmsu.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3veownycz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3qmkktqoz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuhiigzf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3udauwmyy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ggrnxzub.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yonssiwk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ywoeqxtv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3psexdcdj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gmtvbdtn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3xcmujgqm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3dzhfoesm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dbtluuwk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3esytncob.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3koakpwjv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mkjkydzt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3izgpohik.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3yrezlgwc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tujnssfu.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ivrthenc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ebndnwru.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3xkwijflg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3fuawulps.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3deuixvsb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3dincujmo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xjorcrgb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gyfbitca.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3fnajkomc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gohwlsal.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3cyfoamxq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3lempyung.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mkujgswx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ogqssxax.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jxijnpei.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3fhxqiomw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rlqnvodp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3lralmvus.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3rbdneebs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3meuewxcq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rddkprgj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lesyiavm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cmhwpyxx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3lbvpcluh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3oqpzicbs.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3isrfknwn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3mqhjjyhz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3wtzjpgta.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3esmdgobd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3wntgteja.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rxszeykl.html


<!-- 参考信息 -->