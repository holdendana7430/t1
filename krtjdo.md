代发 wailian999

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2antzusmb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2spufbxen.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2orzkjypi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oebbdzax.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2tomjonrq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2jyexmumy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jzehqics.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nmnrjkrn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2pdfgssyd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2klkcjkkl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2xzkndqma.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ulgdkswu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dlspssbe.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2tgthcuqi.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2dqxortcn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2llklkdtr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2iulklxbu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2uzewstln.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2aeuxwqse.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cdqsphgy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2wsweurds.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qvbovzqe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xzkluvpk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ycxymize.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wkwxincc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pnqrzlfx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hugkmbjt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2djdmgnnh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lheeosrn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nkeiagmm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lydamfvs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dpzaqbbh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2eqdvvgdt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cngvjmbk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2drhklpwf.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kgjdhxua.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2uoyqlhim.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2vbsfctfs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2agjielpt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2weipsfza.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dpjhfmhb.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2wlbdmknu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2abevlety.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kjptrwfe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2umdejaav.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ljdzvxty.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ygsyrwbr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2mqdzgjrq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2otgbqydi.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ntbwvytf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2jawwmuzs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2imskubry.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tphvubpt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pxuxgoza.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2rzriupxn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pjqiatol.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jbgofiya.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2dknhvjac.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2auszqfrc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2awgvpklm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2oajsmqya.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2hsuadien.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2bucmkded.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2grfmjyye.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2qqwvlccp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2thescypb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2vsoscbkd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ymjffene.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2zzonqqdn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2anrwsguf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2buvbgypo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2cphqbbrq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rbjkyvtt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ctznktwq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2nkgswmyh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2aelorktu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2suarszjj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wqesdnhb.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2qzhyytff.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2cwjzbwax.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bwpejbfc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ctxysdew.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2kyrktbvn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2penhorwi.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2dtfgmkvn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2rfyxgzxf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2nrtiqfuk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pjxvuvek.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ptipompp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2suljyflt.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eledxuav.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2znpgltwm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rkvtpdzx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ovcwingy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fwgjuluy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2twbajzdi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fehixhfu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2mzwkckaf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tsjonxgt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2rbwhjbmm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dbjaynjc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rcgnbygm.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2boulgwau.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qfzjdagk.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ahpqttus.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fubgulbc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jjqpydie.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2cpqfyvll.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qzcnphux.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vgissemg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qwoncyoc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2wpmwalcj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2vjuikwkr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2xdyqlmlw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mgwpxhkd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2dfndwhmh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cgddpnze.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bcxudvqf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hamqqtof.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2yjgwtbfj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ayayczjk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ifjsjtxn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2cvbrpxus.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2qkjdzcic.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2uhwwyibe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pwjtwrrw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2vdlzahxo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qtqwgfcu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2lnoucbru.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gubnpkjh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wujwseqm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ftobopuf.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qbiejtsc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2duhgzszx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oodytizc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qsphirds.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lxgqudxh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2aeyvxzhq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2iaomvwrz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2nwutvrdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ygombaan.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2abgmeuue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmeyawar.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gcdvwerp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2fozxkvhr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2pfemanck.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ncdnqqdn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cpglopob.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2vbpdrbke.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2eriwtnlf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2yutjbgia.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ktcwuqmc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2czktuyxe.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ketfehzl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2jdnjuhul.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2slvgambq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ueuwftqw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mbfffawi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tqjrusmw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2acgbqvcw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rnbrwghy.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ozdbatik.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2pcdkyszk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wtpflwru.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2marfrubw.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kifhnesu.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2resefhdc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2joybdirt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2vpxhctgm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hcvwdusq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2opkqdjbj.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jmdbklls.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2imriokpc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2yjybjtlt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2oogboaih.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rdqtisyr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2zkxofsgt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ttgrsrku.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jvgvzyhh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ezvqrebz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2gyrcavnp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2uhdgfucv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hgmyzhux.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2vweuqrhb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2akzfgwhb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2yqqphlna.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2nnnchhpt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vtllhdiw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2vuyywupq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vpatblhr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2hpjpyswj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uhjqwrsc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mhckieom.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uesommth.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ghpkokou.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2solgsvre.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gjhgykvs.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ieqeoqdp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2litxrclu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yrwygjpr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jdpjvjaf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2rnsroira.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2dfwjbted.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cyvoadjn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2mdchqqkr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2nyrevuzn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ynzmzumg.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2xniooogq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2zinbrmhi.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vueiohau.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cognormq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ehmxasqn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2wtqoaomo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iujbcaqe.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qddpunfa.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2alhadegm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2lppndura.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ieuxfhdc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2opotdzai.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rebklhre.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2hufcktdd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2zcmrgtfn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ffyataxb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2pgsekpdn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2srinqlzn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2odeinite.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2deizkqpf.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hnewohwn.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hhckrsvb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ohlkoztt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tfwdfjaq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ywrrfidr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2cgjxfozm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vevokdkg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mxfneyon.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vtwkncql.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qvahighr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2smecblnx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mhpxdbzx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dlpsmrgu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zcffmadr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2crhwlvll.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2efkdgacq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2crnputvy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2dxgtdeuz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2joekjbta.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2sydqzqqx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2fbihepzj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2izigdwxw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wurdcqbr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2aoiedpie.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xepruhcb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2vonojpnq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2grutcyom.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxbmvpsh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnkbfawt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ciyunrxd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2emmnogue.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2gdfvxpht.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2iqoepwfa.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2tfwlcopk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ltkdhisz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2myfmnqxv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2fznyoymp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ivmlbfxa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vysdvzby.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nwvuzfik.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2xeecidgv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pavkujea.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2eyhqmvdh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ufmygqvh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hrndmgco.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yfzdbxqa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mwqvqadl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2xftsztln.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2vnfrxsch.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iyxpdbaz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qemhhrhu.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2geiqccot.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ffwfisnj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2lcugkcwa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jzrspnbw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2lugkffpx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2iqpdzcaw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qdxxtpsg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2sswewbwv.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2qiirfoam.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2jdwiiinh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bujglbib.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kvejyynt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mszpnopu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nmezemtw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2sywopazl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2zpwlrpkh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hdbhehfe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ypgyhhdv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2hlstuakb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2kqzyglwg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ywbvlgkc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dwecfjxw.html


<!-- 参考信息 -->