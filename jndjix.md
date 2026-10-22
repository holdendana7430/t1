代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mcnikhkn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ekfxluyl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zzaaxchv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2vzithgrm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wkbqyhvx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sbihjnwd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dmuisoxd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2acohyzju.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xbnzhmhu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cdzgyccp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hfsghizh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mxdfunvj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2begacasz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jaiuqogb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nayeblnv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ckhvofut.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2tiqjayjd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2tqrkfpjd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wfteppfa.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qcdzucmq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cdwivnpo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nxxnkgas.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2porepgyi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gvlfqtfe.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fdpluqra.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2dhvzdeuk.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ntinporv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2voczeiqc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2elsshcvt.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2gafksqcy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2kxdciacc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2arequuum.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2hiqjswvb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uhpfzbhz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ixfxfqaf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2leutdwxx.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2zeoyyfso.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2yedafuka.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2hypnlijr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2zuozeych.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lljcvayq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2sopjcxkv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2eaqsakut.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2byifxxsn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bxzufznr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cpftlrap.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2pyvbylao.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xahazhei.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ulfapwcr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2hqsloxxo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2epxczvzw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2gcupsghx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2wqhfuphj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2zoahmcfv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2qdaypwzi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2hdrxqknr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ciemgqsy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jiolvbwx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bnewpxfo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rltufdoi.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2wijuckbc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2pudfdoao.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2cypykmmf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wbgvvsza.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wszvadak.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zuviogtm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2zesmxjzw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2faqlyghc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ajbgluki.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2cfhzcfic.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2xtzcxpxy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2urzbndhv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gywcqhbb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2telgcfkt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zjsngqsr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2apapmjsf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2fkewgkoe.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2hynpiynr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jlowqyll.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jnalhtdc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2niczrvko.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2svbxkbwk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vtlgvqhr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2odpcckxm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2boesqymk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lmrjcgbu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lsqjgwpu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fqzcgtvi.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2kpatqvuz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ujxtspkn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2eqdrtlcg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ueidwqpl.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2iofnulig.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2jxmoqvwn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2hgnbmaux.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2xodlarrt.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2hqmaazgq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2glnpkknp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fpyibnny.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ibzwwdwe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2utetlhvp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2acgzrvdj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vvccegew.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2mpnkexsj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2bsthrgjg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2wjjsawnk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2tnjlymlf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zbtgygol.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wuybxyaz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ctoipabe.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wfdgwdkg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ueyifhfr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hpvypznm.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2mkkcrzpb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2toxfohjc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2iogwdxpe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2sgjfobzk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2fzlcibci.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zwzawkwu.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2zzdjmdcp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jgzrvgql.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gykpoowg.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2nfciabrl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rbqkouci.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2yjzytooz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ggjjysns.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2jialfkgi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2pedtxxyl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ajkyiyvv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ldzbzila.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2qnolbyhb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2moflfjwy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2wemqerpq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hjxnuxaq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wdimixil.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2cfyjedru.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2sjtleyqy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2czntdcob.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2obqgqrgo.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2qgpeojiu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2dtkgaenj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2iaueelks.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2vqouucyw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dvzuzuhq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2hbsrmjqm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qzndigba.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wajhrqhj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tslcrsii.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vbltowee.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kpngekvf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xgsyzasw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2vbbdghsf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2cmznaxxk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2davhldrz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mfcyegbj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2xpjykbci.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2iwcafhyz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ojhefcey.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2cjxdkdwf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qlshwdnz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2rfhhfzna.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mjgidfhn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2iycpjqjz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2nncbntcn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2krbsmnpk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2nhnktwet.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fxzjsdjo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2dzakkmht.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ldwcpdpa.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ekhzsppq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ytbajrcn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2jasoixab.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2cjoisbzo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zjvrdgeq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2tgpoiady.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2rjoxagke.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ejtotpja.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2lyxygims.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2nprujerq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ucrmqycv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2uwegswnt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ieyrnfjt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2dwxpmhqy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2nndxmhly.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2lomnzeqi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2njmhfnfz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mlhvyxsn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dpwxvkrk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cawnvkbp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xlnctlus.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2novjxuqg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rzleuais.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vyboeiaw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ldlkmutb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lxwfwepx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2foyndswt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zafjxmtd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2xukotwfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ecjxfkuz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jnbtuzkz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ethlvhcj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2lhajedet.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pdvkkeol.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vhyxeacw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2mpvplqmt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2hzzzrwcj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2yuxkbrlz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zlgglzvc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gztratll.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xrgrlqyf.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ziqwvdqk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fsmhcfek.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hjimptvj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xsyzvyic.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2vwhnynga.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lzhjhyhx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2jlhjmzax.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2asjzpskv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2wnphxgat.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fvubpowl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kpyobpkj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2twzxeoch.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bezniyqx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jrizaupu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2xftkilvz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2smmojkko.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2dhmjstfo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lrqnjtrl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2tadcgaqn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2bitcwxjx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tmjqbisn.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rnxjsqkw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2kaolapos.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mefkgouv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dprqxsht.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2yhamohiq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2kejqeayu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jmotpqzi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ychonfmj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2exufinpo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ybvnbmrh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2qckxtfyv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hejsjqhw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2sbedmsnb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ltkzchyi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uwjgmkuc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2umluknrf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cgazwkvb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nzthownd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pmcxijvm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2glmlaceg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ttnhqmja.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2frjryffs.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dijapfaa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2sxrpuvhf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zdebtazx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2aqtreetj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ijxnfvvs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2qxounmqw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2nmvozelm.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2dubceaup.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2nigpqzmk.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2xfujmyfl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2dleupelk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2zxbcupql.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qguvbxub.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xvbvulya.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nsakafxs.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2mjitdbtq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tedgcdxe.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rkwveozu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2qoqqrmxx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2cmdxgkrs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2cokgznrd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ewsourvy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bjwuxnrx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ytzibybf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2edajjorx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2irgswcpw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2esnmksyu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ugtizkeq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lnvzmjte.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hppchfmf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zcrysbcv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bbsfawkp.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2defwrpru.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kxftjutx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pktmwoys.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2wvrdufky.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hrqylfmy.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ufxgihgm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tdsxnjxt.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2umvfyqna.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2utbeazvy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2chkotema.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jwetlkcs.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gmoyuiwb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rmqudhvk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2yapgzfbu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2resdvztz.html


<!-- 参考信息 -->