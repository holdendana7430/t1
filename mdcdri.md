代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2apgygrgc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ghkqtofw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2qdrkenvp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bzawkcot.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rlfktgil.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2dehxjgop.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2wbbybvhe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2kahtwhgk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ivlzudat.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ogjhkyir.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2bbodupnj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2lhnzwfqg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2xxbabylx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2crmlpgbf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2givjesaa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cyllhmpi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2dogptwbb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2dhgnhkhs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2tnjvbzdf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2rdbqnwdb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2rwgaegob.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2urtwvjaa.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2youkqoye.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2mpxnzwhb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2behtfdnz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2cpezlmlr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2umolbngp.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2tpwgpfgz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2eevierdx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2imrksqzu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2wujvmkel.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yegviiap.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eagoqlxl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cmzrwboq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2okucnkki.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kxhquulj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2dchbweqp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ckqbirdm.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2iudfvasl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2aloncctu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2jbbczbll.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nxljnwyq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tfnmwgpr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2uozuowzx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2pjkfnulg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2lbmmotyq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nzfemcwg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2xkdlooqj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2txrfrlpi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pophsskx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jdwkplwb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2pndrwflp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fupouwwm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mlpextrf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jjtoqplf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gumrcoof.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2sxfsypqc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vfyloxnt.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2cnueulvw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pvmmpjzn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kogyxpsl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2bqniqoxo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2fjxbuyku.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ssiyjgxh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2hgkzmwpy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2dvksszyo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2edbemmwu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fvoqsqwh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vnijcaoa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2csvzswcq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2womrqcyv.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2gwhmmkuq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dkbxkdxa.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2zbmsebpk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2xozncawv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xqlnyivd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2lujofenp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hgkyxuuh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2thlqfbvf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xaxdgfdl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sabzdjeb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2guqvnari.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ltlqcdlq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2dbttcjbl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2rnbvzbhc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2pzqqutkb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2qqxbsabe.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2eldxmluy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tkjzosnc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2tyjvuzle.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2iuecnzmq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mdejgcmw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2amamjhid.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lxiyxydh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2mctlbhyb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2waqibpqb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2qjtelfxt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2bgthvytz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2cdsoqiyz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2nhxojsdi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2sadrwhox.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bichnvoo.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hzojiuws.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2auorvpaq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ycormjnl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bkjreucu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2jvwqowmb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2raxebuee.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2kgpkxdxa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2kgovrres.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2xbuumsdp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lmpjobxs.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2edybhtqm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fcwutkvu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rdqdvqhm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jgqziath.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ogdfbhtv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hfgwirps.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjeqfuny.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2jjaupjps.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ydaskseq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2fwwczuqe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eiffkbht.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2toqltqwl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2sewlhrtj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2hudnfagt.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2njxdmuzs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2uarcnqgy.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2qyhnuarn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2eoeyhxxe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2vkpxaowp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2cndskldz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jxijmket.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2zbgjzfxv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2scgucxki.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2tmehhnnb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ydlttjip.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2lqrrbksu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vpaeerlx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2fhwvzlqy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2vfvpfomd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pfsnfzne.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yeeomycr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2pafxrdjp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pqikvfmp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2knznvhtp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2lowvqluh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2dpxiltmp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2yfsfeizz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wedmzcdj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2oybbxwke.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bfnndngz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2blxynkyb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2engromqf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2atuyfeme.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yyxjzxze.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2octtfnwv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pcpuwowe.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2aotcqfcf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2odaitxud.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vxhrkjil.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bfhzwnfu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tltnciwi.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2okzkalea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fybijndz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2mmcaldgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fmimdrbg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jgtzznhd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2mwulpnzq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2gmdgcocy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jcwrynvg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ehnzfemx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2laeuyhof.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rfbnzpkg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2oqlfsokz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mwiegluh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pjuodxjx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2njrzrojk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jdblwrhn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sgoxtrzs.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tjkcihjf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qcdmrodp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2xcmucwcm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ckgjufmm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vimbcqwa.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gavrarhe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2egkrmymh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rpttdedk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2adsplfje.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xqvurvzn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2isrmqajo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2uiggjdxz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2sxxckrxq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2knxzvsuq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2smrijocx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wfemekqb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vamdnkgo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2jayvwmyx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wkpsalpm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hzyvyumg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xmsaafad.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hjdbqaxc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fwitwlhz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2muljmyzr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iluqdguc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ayxxabdj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zdkpjjxh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2jcodfzid.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2sxxfynvx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2xupgdxlh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kxfdvopf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ctngczsw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2wualovjv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mcljmspl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2jxlkzcfa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lveskyex.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tyupwlcx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wgszyobw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lipawchl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qmkrkpxp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rvzkdseg.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2untxjqgt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2kjenlbur.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eiejltnu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2oorktnif.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bghdwnow.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2russieyg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kgbgfywa.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2legtskyz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2rzaecnqd.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2fmrzheyi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2rchepbhj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2gbbdbhcv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jtlvtqxn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pqtxmtgx.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gdvbmiiv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2sjgyicje.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2sfuzxxkd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dplwqwxn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2dbkgmjer.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2axulgyph.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2cjcxnvkv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wcoznbsb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2usgrszxe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wzkjifwx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2jjlesyxq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kfzyivqf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wibynczf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2snbonawd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wvdhukkn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gvdbmdwx.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2galuopwd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fsczjkgw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sfqyzfpu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kzgtxmrr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hirexuei.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2wggqarrx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2omaahghp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dlrspyco.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qhxxpckv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qzsfwxve.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dvynhgxr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sbuazhiq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ohqefzyd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tkhqfywt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cgimkfio.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2hyxcxfjb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2srxrrjxl.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ehtoounk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tjzipztp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jrbodhag.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2vuszolge.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ppattpeu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2tupjlakj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2xwejrkww.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2tjfeykwj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2iicrnuni.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjeamcqq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2eppqsbxd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kqepwvbu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rragwmec.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2dnmqikmk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2rpdzplob.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cnfieowk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2qaweqzmt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2hhdvfezd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qbuajvhj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2cqdtynvm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zanumgrr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dgjmdzhx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2nybsswoa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2rakoyiff.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hviarmiv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2jsrvqade.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kosjhavs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vdsxtvte.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ayybixoj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ziihggcz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2zhqdwzwt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zkqequal.html


<!-- 参考信息 -->