代发 wailian999

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hsorghmm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xocnpcap.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2lcwyygrk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2uzuavdia.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2odwgsczm.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bwldfgqv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cubitzzk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sxbcjokn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2opdxsbpa.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2phbkltdy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rhmemvwp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ddfvdapd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bgqrlvqe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mwlmazyb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2rtcaysgb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xlcvajox.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ytmjbnyz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2uzkhgbwl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ktebpmmm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tvtmvbkl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hrektzvo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ezjwmauk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2yvgwznku.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bygipitq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ahsejyso.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2pkwvagxo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2cipcmjpn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2behtbwdp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2coevmgrk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2almwjqss.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bwuhazuf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2tjrjyqrg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2gtljsxkh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xvupelnb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2gqsvaamz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2wzpmoyho.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2gfnornvo.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2spskqtin.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wtsryfuu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bvathcxp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ybwduruc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vvwpayfq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2epjvanhn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2clifgmfy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vonnxpuf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2dwnvlyfa.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vlsryrzi.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2uorjlqll.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2tuvfjcpc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2bifjpqmj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mpxlxvsk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2nvtucbfo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2uvwavfwd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2eweajitu.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2hyisijfu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wxpfrtlj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ezqjbsnl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2quvnbbyo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2aqvvdsek.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2grrxjbju.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2urtoyjxc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2faxxqozh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2fpmorlxt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2buriuppv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2xfrjpenw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2rastophc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2zwgjtzhm.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2xjkimcuo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2noxdvntz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ewwanzmh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2cylbmqmj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ivrxbnjg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2lyjiekqj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2aesqqfno.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2rxubvwvx.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dnwaidfc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2fpoqafht.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2emizavwj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dgozajgh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yxnpenyx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qzzlzfrx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ufeicmfn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2icaxmjuf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2poyjkuvg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2kfbhpgji.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2dvfpgnjr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cozjvhtb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2yoaxahfp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ivpfeeiw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mnzjtjew.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2qtmiqiuu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2enxxumap.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2opzmvbww.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gwtkwdqd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2nzqgdmgc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tvyzvfik.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2josoqews.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2esbjluoa.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jxyyroul.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2moiwyjls.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2hdwwuzeg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2zvlnercd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2knzdyubv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2zkoibanq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2glghikiy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2whqgbmxm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2fahdkmbp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2yrcgricl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2xwbfyzyu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2cwpotztg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ufwefoyj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2rnbolihf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hokmvree.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2drebzkab.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xqfjdczs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mptmqeto.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2bmonmajd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2dpgihpuy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2igdlkhlb.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2doircmve.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cfhtoaab.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dpyipifr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ugnvexev.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uvkqfeie.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zazhczhd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2egfdddut.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2visjrwhz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2oiimiilw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gbvsgrvx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ttsuyyof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dgbmuxku.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lngckgst.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2smppmtll.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2tzpfwmwq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qpvzsaly.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2crdqdyfy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ocesdndr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2hyhcphln.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2sppmudge.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kyrmoymt.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ewctyhpg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2swcgtktw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ehqcgand.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2snssssqr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dmgdtpby.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cfxmtprc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jotyrdow.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2duhrtxjh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2tlsswqtt.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qwrccjxk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2vevecgsg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nuwvvlnp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zqwmhuhu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qbrbygti.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dljthazq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2srsqcmht.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2biaytmqp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cwvtsjeg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2lwtytknv.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tqbzcsmr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2xedjpsqc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ymghyoos.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vncseldr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2spabubzg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2mvyoewci.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rggznlje.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xfivxehc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ahpomwux.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jmuiiiav.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jsubdetg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yonqvhop.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nyiyjmfq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zrsbzyqd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2gqtkldxy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bzsmkeob.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2csatclwa.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2xpkepaoh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cbviesxo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ectmdnab.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hhzkvfqj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tbexrzwz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hemsnofg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vtveprmf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wlmlvcta.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jliurozm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2sfquxamg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2vmihzjwo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sgrkjywt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2dkgaxkph.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2svthtdel.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2udcptsoy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ppkovwrn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2gctcicvy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2zojzbyvg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2pctkjklo.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2bigepmho.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2brnfsqps.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xukjlnzx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gfspaaqj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2sskzxlso.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2gitkbcrl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qhcumwzu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lpamsowb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2yioyjbpd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2qqqpwjkx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2xngawrwu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ecrfjgjl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2swsurett.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2oxlqjxpe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2zalxtxqu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tzqbevpf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vttoffwu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2xitgwcyw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ttlyvvaa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2dzlbmibh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lfxqwnig.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2goghwxrj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jykdglqf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jszstpii.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qxzrvyyt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2zadpcnyi.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2rqjrjcyw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jeyrgkno.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vhfytxnn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sdxuiyku.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2khmwdffp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2rwvsonyb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yekbnxjx.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kvqwbyvm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2aykokrmp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ztraomsu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2imtdkaco.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ztoacram.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vsleyjpe.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2egpvhqye.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2czemayda.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2rzqgrgwp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qxwgxxsb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2nmhhertu.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2rsjdgwum.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ahjynirt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2rppwovvo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2adjlvooe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqlnazns.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cztaxfpb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2zdkggsfo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2tmhinpzi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sdpidlro.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2lvoemjks.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2hrtouhkj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2aifmwqxb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qwyqmdoh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gwthntsw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cenaoakr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2etsiiwdu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2yykvznor.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hodrmrcx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2zerpfqyw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2togentdn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hykdbkvy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gbcddsgh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vntiulsb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ccidwopc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bjdjcxhg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qcynujld.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yznxnddy.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ldwoxwug.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2jfngqgha.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2lerwidyg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ccmlpfad.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ueznkkkp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2uzyjdhaz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2gnvaukpr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uaivngfn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2smuttzkf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2sbedltzz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ceutsnqx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2mluwbrwr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2omieedjb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hrbjenet.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jxcnerzk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2vdswgucr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2rhxbqsgc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ezsmtccf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2erlonznp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2gjvuwete.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2kefgnnfm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sthgjygt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qqtyhymn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nopwkcfb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2oxqqsmkw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tfmpojhv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2lymsofqb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ujyqerya.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2gqzrvrcw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lmgfzdzp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vaymzbed.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fmxbntqe.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2lpamcayc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2murksywa.html


<!-- 参考信息 -->