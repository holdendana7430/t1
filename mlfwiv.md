代发 wailian999

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ykkrhxna.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2rxbdzczg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2sphbnasl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2qdofnldw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2gsjwgdvq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lzjaqzwu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vwkasaml.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ysqqnybi.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zqkfajbd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2yhcvuvga.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2brozotie.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ehvkrebl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vnfgouht.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dgqfucqn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2cdqiwiak.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ultniyuu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hdpmbpch.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2iveuhepw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2agujwhzp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2npwfeoui.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2negqhpnf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iezxulwe.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lrwuavkt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2oxuvaatc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2khpiuyxe.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2astahwgu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vjmgfvgx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2awklvswq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ikjwofro.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ctxfhpdo.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yasgfjio.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jigbkqjn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2wnmqavsl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2oxjyabfh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lxcmkqgo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dozufxcq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wjnzcefm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ohrqtmve.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ilkdffsm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2moihdxmf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ntcjsyxp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2rjjlppkb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2pepujxbn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2diigwzrx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2hgjptnnq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2loxouefu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2amkchalt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wypjzbqe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vlnbepnj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ctzrxdvl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2mkqgemzb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2gihcigyc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ljtqzybe.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2otaybroh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xipvvomm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ehjkfcds.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2lmiitblc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2wwizdzqu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2feobtowe.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2aadnnusk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ipgwkdld.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2pvljaldf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2gmxgjowr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2gpurbzog.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2eupqkomh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2yvhvsstx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2dlppkjlu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2zbdcuijc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2iuocmipk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2vokscgyp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2wkcwxihc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cuxnlmzs.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2nryzhvtt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ydeyxluq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2sjzzlxco.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2etjnoqml.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yrzhoift.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2lnbqpjjf.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2jclaumjx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2gjzcfeyi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2qntcbjtx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2vcynuzrr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2tazymgqk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2zshlpxhi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vmcymtqz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vtzozlxl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2mbqkinep.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vfmicdky.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2qgukvbcm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2amsoqafc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2gwkcxknk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ukgdoott.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2yqzfopga.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2frhnqtuc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2czhdgojh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ujngplme.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2klgcdruw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ldbqdepa.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ijkppoeb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2stvwldes.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2rbbwvqip.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2dhvkekkl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2tpiqgitx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2fwcmumab.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nsqgsjlu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dpbhliod.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ycvbqfdb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2drjerzmw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2svjjkjzr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gnexlwkm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xhdvnurj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2koaxxtqg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dhtvachk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2awgalvxd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xgkhmdfm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2uoactzqh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2culwjpfa.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xuyjkjqr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qpxybglt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2stnbondp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ntgtzhvj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hjcrmrkv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2erqhnoef.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2eydoziui.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2msucyccf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2zkbmsbkg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2rssuxrdl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2rttynkmr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rfuhuljp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rgqnfeer.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2uorifbxz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vhoidbuj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2hbepognr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ormpiifz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wavmmyja.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vgcqutrg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2infdzjur.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2slmgyydd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hjxxgeyq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mwqjwjaj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fvimpade.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2olpfsfbc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ztgklxbu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nojwahad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wnkkgjbr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2fpvlvuuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tocrpdjp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xqqjlbzk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2xiitfzyv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2zriiewdn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hilpwovq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ojbpenaa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2mzlxgioh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2diayjvgz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2bguuwhfg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lydhqluk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2yroczsgb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dwrgpeiw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qksxusgy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2datpomco.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cjfsoyms.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zqoamwao.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2uddmwfld.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rolrtfpn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hvludryd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jczqsimz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2nwktbeur.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qhhthhpz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kssisgaq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2odlkhfkh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pnhbvmkn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wmnzeeti.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2talduzks.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2aywwdxzf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2udnhbmrt.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dazfxaya.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ttowbpvc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2pbvbibpt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sgukonyv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yujwmhle.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2kuxrvbcq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ewhqsjil.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iyzenrxr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2zwdghrha.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ucmpgyyz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2emcrcnbm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xkgxqsfu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2uwhvotbg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jjhbnlda.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2tncbmfsg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2rshqmgmb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rvixgmfq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2gfnxethu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2yqafhfdx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2yrbsiqnu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gugezewz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2chrpvlfs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iryilpsc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jlwrxntw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ocahpbml.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rrjeucpa.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jxzjdmwx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2idwllbkw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vtuwgdiv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wwpnkyzd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2whifurob.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2witgfdzf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ffzpblnf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2lrqeiinn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2jxeofchv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2cqhssvoq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2uflpqmfd.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2qjyytwwc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nhbqguyy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mrzsccaf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2oumjssuf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2zvidvqjz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2oyvglnsm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2awpdggmw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2wvcnhkrg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ygmnrmml.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2myuuoaxw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hxdopiju.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mvtyjbol.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dclxipwe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2hcpacldh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2lyybegnb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2eirthhxn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2etrlorqf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zkrieuer.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2bltklnsf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2forccpad.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yhqzmmhx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gsftemhp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sorakgwg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ynxwvzml.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2jihcipbv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2uokkfxyb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2gfddflov.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gwfwxcoe.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hguapwmg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aeopptjb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tzqktjfe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2mqmrlfnr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2egzddrfq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dubtqtgn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2bbymttpo.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rmcwgsju.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2dvnpwdfg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zqpuyxdo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ymtmvttk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2noxpnodz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2egtamvpd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jucsokvt.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2itqzsfiv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2pwwihafx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2kjaofhbh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwgvwkuw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpsyhgjr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxpqfezb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2emyqcdsj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2dqppqdtu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2hbywpkir.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2evuhdiiz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2teowtdlr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2flhaewzy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2snrlcfcx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2xuwlzbbc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ythevfik.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mnkgdhgc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2kddtkyzy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2hzekfckr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rljowmkx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2vofyhkfn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2whlzlamy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2kdlvezor.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nahvxneo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wlgnmgsr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ylyujuxi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xvkbcezq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2khgnyamf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2unyvsrsk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ovoivgde.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zqipybbr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2lricwwjx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2rwtrbdki.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2woqnwbqd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qcsqnyzb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2avmwuwll.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2veipnldy.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2jofflgtf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2kuzqbvan.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2cjgqsnph.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dyjbzick.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cfngkuda.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lhaxaqvr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2hrgoqkto.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mwisalhy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wafwgdrz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2jnfmxvfl.html


<!-- 参考信息 -->