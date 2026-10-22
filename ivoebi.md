代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2jimdtrfo.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ynemxuxd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2mtnquoqx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tviavupk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2jjbgsfgy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2nsuglanq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2omvbiqcg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2wrbvvohf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zhpncgcm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ebdkotaj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2mcbniquy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2bvhpxosh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fsitrrbp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zvzjzsid.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2uvwckqgl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qopzzxle.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2vkgqwjzh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2dskeyoog.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2nfqjntbm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2tllwfjri.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2bvlguhxt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2nbhsoily.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vgaobjeh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2gymonxcb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cynmhtxv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vrxcnrgf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yofhrklu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2uglqzoxu.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2nmqdkkhk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2yivmyrqs.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2aexvjtwp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2drjgflxz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pdvyoqwy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pexprrjy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2tzygjbtm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ltaigtxc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sbikuvwf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2hhbzdels.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2koxrvjjo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2kkxztttu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hxamgvip.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fbefdbvn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kaaslsmh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2phsjeuap.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2tmjtemhd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2cgablsqp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iwoqlsio.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2nowyoqeu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uxpzdymy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xwdxqviu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gtvxiykt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zftxcyel.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2cfbzyrtt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2uecvbsgi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sozscwjb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gqfvtgof.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ztnsmsku.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dpkwlmqy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2blylcvki.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nnsldmwy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yzlmgvoc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fuwoazrp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2dtdloynu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ikzeflqm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2toutatmg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2wlsldfmt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jueqdyxa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uzbnsutl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jjftxlgg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dclsmxnz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2xihvdaax.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2gxxdfdfj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zvaaoxli.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2szkjreyc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qifywkoj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2afhjghwo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rkexdeid.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2tlznnzkj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2srflupxl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2uufwhczv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qiqglsjz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2enrsxxbv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2yytbyvac.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ecmgunlq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2rzrhayet.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2bqbedads.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ylzzsqph.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2qqwpexiw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zikmcafy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2qimpezpl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2eurtvtou.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tyhyjehf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2azhwknsb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ktckcgts.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2mkjhcesf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2kfnyuboi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cvfxgywq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2mmqfuehv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2yiseonsd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2xnxxitwv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2fsiwvslw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2glcsrpwq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2odlajxyb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2fyhqiqsq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pspqnput.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2oxtopxwp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2cgwdlpsn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2tplnlttw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2tsrbjeay.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2dfqaczef.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ixwuiksr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2uvuvmlih.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2heeycjjp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yymuaxpt.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cscuvlay.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ldjzgmgy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2soibwisg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kuwqphfx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ealxpmpt.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2mruloogb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2avtwynmb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2orkkqvkc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wbkvupyw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2jtrsemdi.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2lvbscluj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2rzjwbgty.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ahiyzgng.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2zvrabppq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2nudnrtsc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2lmhgbwne.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yuyzosqt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gtlxdxhn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2twfbhmrk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2xwynltwa.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jticikxt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2rqryjfpg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2gisoxewe.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2yvodevfn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2tsorjdhy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qiakpedb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2zdmbayqr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bclpuozt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gfyvatvj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2guhndzpr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ersrvmrn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2tuxwxabq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2cvnfiolp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2rpibotwk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2plzjhnai.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2etbzxplw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2kcncgffn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dngukdqx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2wxkmbfdh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2hxqggsss.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2glioavwd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2gqpuxjon.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iltxvhtz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xalgoidx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2iorbenbo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wavjhsxd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bghcoufn.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oztmlcan.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mqvvfdbb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2enbnqxrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtasahay.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2xjceqohk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akjtqvmj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lhuvlhkg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ngwbklbx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gcbdhmsy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pleybmrk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2azzvfryt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2gkhpaxsz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qeyglifv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2fiuoxmwo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gdqqnbsq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kvrpfjhn.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jdwagtcq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rerkfgou.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xgarpeee.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zbgkieqp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nldarulv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ucqypcyq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2znypdlxm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2hojzuzag.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2uceexhok.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2hitkqukp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eszwzpdv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wkqtunpb.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2elgsowwn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ftacfqdg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pcepmjka.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2spnjvjea.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2jiwjjync.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2vknvnggo.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wpprkqvp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2wbpkdisz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2dsedtjxl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2anypllnc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mozioama.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2kcwotyzc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tfksykcd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uhqmjeic.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2yramtjrg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2labjutyu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ujfbmeby.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zjaawaxz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2rpqkzyvx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2arcjmiza.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2khxvgtzm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2hbhfumxy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tdsvzkbi.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2jbquvhxt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ggouyucm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wqfxpdmu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tlzbupix.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aryrvnsx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bqeonlbg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2toddqsvu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lzpgxkzo.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bwuerexs.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2txirlwxq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2poytazpn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2baetjuzm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fjlfrlql.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2eaiighoj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2igjvtnoi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2yoesbdnq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2jnirodvt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2yvprztac.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2yefgltvx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2dmbidkhz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2xhdbqpae.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2krrywxxu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qnrlnzlv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gkerbhle.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2anguvzcz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hoxugwso.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2efksuiyn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ugcynlzq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2sqmbqxdy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ipfmbhmn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pkapgumn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mnuuhqxf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2fgokpdpu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2inglkthm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2klbbzdxi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2khvvgvcb.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2pnwjftrb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bejzcfys.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2blnmsoxz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2aglgpgee.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qalcfrba.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dmndwbyl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rppjobdu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nhtampfo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2rcrvvgme.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2navwtcat.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2iovktlbe.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yzrtgxhu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fedzrevi.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tpyhejfn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2etykgpjv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xmrayesg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2filzgzdb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2fxgvjcnh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2trpixtri.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2icekihta.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2amemidvb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vvhdrrdw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2szhpvxgz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2xmtmymcz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ovvzljqx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gooklqhz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2jrreevgx.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qxvudoro.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2jhenwbrx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2imsfkhnx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibmedvuo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fwhayprx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2sekexdiv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2abkshlox.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2hwpiyhrq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwwcenxn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ynedrjef.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2prklngih.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2rfrpuzlx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2urvhdpjr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tjggdvjx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2znduwovm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ssgdltgo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2fkzwudby.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2yymqkeyc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2xczuqudx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2opaddcah.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2lsyuyahy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2mcqqsngv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2epssdzzu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2tvfaoeey.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2lryphxnw.html


<!-- 参考信息 -->