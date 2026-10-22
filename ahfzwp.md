代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2cvgccldc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2fvshxnzf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2cfykgewq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ohnagvwr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2wrsocxht.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2hmghalzd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xvamnolw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2pyqozagx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wplgrmup.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hcewezlz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wfhqjzpk.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2vskbxdly.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2mowispqu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2wjkmuczi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vneibdqa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jwmhtgxn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jvvywdum.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2afgddnrk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2lrbzqvah.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hlroqtwh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2xhydagjx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2shuknwnb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2nqpkgpaj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2keliwqof.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2adibeieq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2brkwpznr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vrlvshvf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2zscbxqmw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2vluqifqh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ktucrtcq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ugpaitwx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2zvodgbqt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2itjdhduf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mpfekkvc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hgnksdah.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2onsjwgen.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ckzvaspg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xbjdtzwz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2prpibhga.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tirkuvpe.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2eldwqfnn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uspdjiec.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2navwlgao.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hzuyaluh.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gscamzzp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2vwpiacbg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2agnxttiy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2lcgfbbes.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2nppvsigb.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2cuwxmqqj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hffeoxrd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2eekigkbr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ftzgrzub.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fmlioiwr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2znhhqptc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2feypvugm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tvmgfxkz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2nwciaumd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vusdqrpg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ozqmbaii.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2cwvdblml.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gpulfusw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ldmjtumh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mistegyr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2stvbwbbd.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2jhnxbdcl.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2nrpzvzfg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2xqqucmtd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2nynrutip.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ovsksqro.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2zegylkhm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vuxyqceo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mhkgtodp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2kwjpdajf.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2eldzqdvv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cseuyrfc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2bvocglcl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hsrndjwx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2euhehnlp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wyrrypql.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2flhfoexr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ncahohtr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2pluxsumo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2fqcihueq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2isbgxgms.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2enyttlxm.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2zivebcyk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qjdjsgyr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zbzjfrid.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hpgdpnyk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ofiukmlu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2dmrusklj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2rhvzabjw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ysvkmgpq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2fhoqknnr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wavnezzc.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zqbwcmgk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ytknaiqw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bltpcmnf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2snlgkqhd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kncdmfkt.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrhrvnjz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2niuailqn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2qkpmaako.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ajtggksc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2fjqvhmuy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2szeroomi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2trxudqgy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ldtjhyru.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2rnbkouof.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2clupgewy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2lidqjpsa.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ajrsucoo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2szpsvpmx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2cbrmqckv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xqdnedgj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2odwtijhu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2hvdmyisf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xvpvqqcl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2zpaybdbo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2aeiibleo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2fxbgdfou.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2mtrygzry.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qrtwhqrn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xsresnox.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vmvtrusj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2glpvohzw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2qajzsmeq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qvdldsvm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ydpafklh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2qnytppey.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2wdtmojho.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2dsrncxtt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bgsyktig.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2tedyedvy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jzkgohmh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2mitvlxdy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2sqmduhkh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2olxhascw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2saqszkvc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2yjcrspaz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bqxsesij.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2eeauccuf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jspycupp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2pvjfxoni.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zvktkhmx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ypmnifze.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2piapsagp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmexybpo.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2nphohchb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hnfsbhnm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dozdlslw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2vckwlgoe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2fexcbxtg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qyqzwwfz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hmxfgyvl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jyjijjnc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nuzpnlrl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ynhntrxe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uxcioqoz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gcvonnlj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2uxcrepqz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kvxfolsv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xizmobzi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2youupndm.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lsuqbkzz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2efxnwhpb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2oyxwiwyu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vmsrqrhp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rsatwlln.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2devscrvx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2symwxuzi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dawryohj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2eljkzvlv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2luaggaya.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2uiuhumxt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ncolgdjp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jwrvoyok.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2fivppwya.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2opybjlkx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2djbpbcbj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2dcadeqgv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zwyvvhtk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zpqgtzrw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2vzsvwsrs.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vzrvzhkq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jvyilfmp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2mpbvubny.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2lngumnmt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2cesbvdvt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wuyolqou.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2pvmjurdb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gmzutkhk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2zwrxtetg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2btqmotej.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nhndatwb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2dhncdinm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mhttuwfw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2rlhshmgg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rwdqpulh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qtlcpwzt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vrbsnwde.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oiogsipa.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nfpqgdhc.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xocfwkxp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2iiogxkch.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2dtvtyifa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2supnzqol.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jhdxxgbg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cvilnzfl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ioipxqmq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qqmbgcgf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wyslnjtt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2srghrjkz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2bwlxddmt.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vtbzwgyv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2nhdndtyq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2iwwovhdq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2djlbbiku.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2squechbo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2zharbkxo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2foxjsvlv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rugttxpo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2zxfuqvjq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jszvcapk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zkuhegnf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tdrelkkj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ojftptse.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2yezfcpys.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2sndcuszy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2qclbuphu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2svsbneuj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zvzumurr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zeftiopl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2pndimzco.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kljzddhi.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qzipbjem.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ddpbczwk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2iamtefgv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dvhntjsj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2vreblbzf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sgloohtd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rxfxefcu.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2niwlywhb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ntfvdlmg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jjyulryj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xemslvmt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jokdvqzl.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2wjnocirt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wnlhbzid.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ayrxreap.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uvxmaamt.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2hxgrwsjb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2tlgbygqe.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2aaclgwyr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2pvypywol.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xuomfing.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2sctpbens.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ldusbetz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2plyywzvo.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2wdisgapm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2tscxrxuj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwwdirqt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kwczqmfm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nyeazyou.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rzypkvnr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2oduxsvmt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpticegg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2dkvolnsa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2fuqzizji.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sdivpaia.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2wghljmkk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2oejrcnzr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mmoxcbzu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2txekasyl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2tpgvjwlc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2badbbohr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2srazryrv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2zbslcdyb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2wolpymmy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2jxtlqutt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jsrkwqrn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ilaikhmw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2lzqlrzpx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2tnuxgtvd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2xybuxqbf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2awedizmw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2maqnqlfj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2dtfsjnzp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cmldtubd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yvgaluno.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qjbdnbpz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2fukcwffm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rdwtejqj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nxjrsjob.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2vavjpnkf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vdxoubwu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qebuzesf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xgzzkagy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ujcosjif.html


<!-- 参考信息 -->