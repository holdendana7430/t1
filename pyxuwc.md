代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ydevpldb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2dagegwji.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2oezmcspv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2jsgikjvl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2odxslthy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2unighygo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hbznehme.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2kusewvsr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2odvhjcmv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hsdpozqu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2fopjjgdp.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2pkurbytv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2kniwbsrh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ptawzzwo.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kxsrwvtt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2veggfiaq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zjkdryip.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tewzikna.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2cgilxbun.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2imipwzrm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2esxkxlep.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ywvcugwu.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2kxgshkfj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2wqschiuq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vnlohwcj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zdhcvmyv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nhsapefp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bspfplgh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2lonkjgcj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2uaslmwgq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vxjwzdbh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2cjbdhgps.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2wsinxnyw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ivgabuew.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvuwfvvz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2duaubvfk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tqizcrkz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nyybqyzl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nsbeinjv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tmpirorr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ftbykdxd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rpzsynna.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2hnrncyaa.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mhqcuipz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xqwrodce.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2tecfptfx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2uscgnesi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2scunfevp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jpcjoesv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2eiqtvhfw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vzknpdwm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ztkvwuns.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tbbcpddt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jvggzvle.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2otovoawp.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2tcubmayi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qnxcgtrv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2niqbryrs.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2bkaliyvm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vbxchhac.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fehukncz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vaeyupxu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2nnlapshg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2elllayeh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ozavdzkf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2puwusunt.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2iwmlfjzz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2rfrvuihy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2coucdcrx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2bjfvdemp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mpofayhs.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2hzcorlic.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mdiekran.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2cxvzdfsd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2qmcbuvsa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pfcqsdmg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ltijjrje.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2lniwysfp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2jduvokpz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2betkznpj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xhwzkfaa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2whtexgzi.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2vsmatanr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ftkfyfoa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2cmtgujny.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2skcuakvj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2cbadvuol.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2urkhnubk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ouyfxnvx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2eulwgtgb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2evunxulv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2yzkdhbgr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2zcigzjcx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ybpigjkw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ygxquadb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2jdyvviup.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2gqxdhclq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nfsibxhh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wxsmdxbi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vofpdklr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zcjmctyf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2siikaemp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jqfhexqa.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2yzlcftur.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2nroopfmr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2shxffqlq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qleiqylz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2sfohjdbx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2mtldtqzm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2khulosmn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2prqnbioy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2xyegehlw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2nqquwzub.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2boclhtnj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vdypwcrk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dodvnuxx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ajmezder.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2szcdvdbb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2iariqbrr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2gytnxxxv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2bcvjjmia.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2bbaxshwt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yjkxybbt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dbizconf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2lsyatctg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ogpgygpc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jywtktov.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2abfumbzd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dlbyoids.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2deutpkek.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2wlaaukvv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ezvxqxgm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vuxzmplt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2uwxhwbgr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2nvdtsmxg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kngwdssa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2zhksnncp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2yjwbaowe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ybytdqjg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jfgpzygk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2rmsmjrrm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ymjqfrss.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zmvqmmzv.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rgoodlcx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ouuziwnw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2qovpiimf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2odcddvaw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2puiurjrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckrywwep.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ekjtphnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zlsyogsg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fhzsgwew.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2hludpwdh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2tbiqepzq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2amuroaer.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2awjqzvds.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2fqsxgodq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qptpzqsg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2yhchpapi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2inyvzwuf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ucghuxum.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zzqznbsr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2efrqvqyg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2krvcttlr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cuwehpkl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qhbvsdby.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2snzhyzkm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hhctgyty.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vbwvwzvo.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2mtpkeehb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2gjmlgsiu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lxpcebsk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qscnzafk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ehiecolz.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jaawjrig.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ddjdticr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2qfalblze.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iylqpacu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2pzhgdsem.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2eegbgvbh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2vvqhqmuj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2kfrbxuyq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hodoltik.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qciyutjq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2licsmrrn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ghyadvvd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iuzeduct.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2lfcldnvd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2obzutqrc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2phjndxke.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2eqopbkyn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2yenqbafh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xqtxhxgr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2rcetqhji.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2nkrorbfr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qiijsgzv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ngboydxq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hytkzvkd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2micwrrac.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sllcysxi.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rdiaekmo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qdhgdmyg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tiuzjziy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hquagbur.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qbkkdqdl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xzhkqbex.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2bukkxlcs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fygpimqn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2chvonyme.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fdvhplbl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jzqqikps.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2caukfglk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2oylrfipw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2kwferjxs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2gplfvmgq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2roqfebik.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2optzgvsz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ekcimqin.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kxaqyaxn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hseeqzna.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2xedomqfy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gejmpsyv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mzvyypfj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2nevotauv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cnzvrpfz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2bryblxob.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qtcldume.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2auagazdu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jkahtbar.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2bxrypljq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fknnbpom.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2edoscsvu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ynccfenv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vqlvopxd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gyuqjccn.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hwjsaoug.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nbxtytoe.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tjqahkuj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vvemddxc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wskxvusk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2kauhldad.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2skftzctz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wxtlbrjx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eqabknpm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ghhvczgx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bsdkjyey.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tcmgmxzp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ynecffyt.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yuftolml.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pnltbgpv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2fywiwryp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ynovhrdd.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ukauvmwz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vkqylrit.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2udrkhgph.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ckvmblbg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2dkcfacyt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2sfrduddy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2tkwfirhb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zjekoqqv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2flsehegg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfmuwgyp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2iutjigge.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzyafsej.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rxevmipx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zvczkted.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2kpsrfjqw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hevoxdvt.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2vacgepnd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2kqxocvyt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2edsdtbpg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2zvhpunsv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2vrqkuuwc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nmikhkxe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ufcrassq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2nowisknn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ngwdlznm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2igpjqnyg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2kkpzvkkp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2shypnzye.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ipwczwkw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2jrdnhzgf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2gavgjxnq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zykjtymp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2xtunqcci.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yysrtiiu.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xxwvgfxo.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2drvnzbtv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jabcjycs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vyxhipqa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2rprgurzk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2blsifabn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2pvgjkeet.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ynmeckia.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2tsszikpo.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2hekjimmi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2pjjkkwki.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2nttsoffa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2oheupkqk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qqncxnan.html


<!-- 参考信息 -->