代发 wailian999

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2yiskscxx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2hyrexfhl.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2aeejoyjk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2sovgvjli.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2awwxeuem.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2lsczjdoo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2isssnvvw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2jwtqxlxp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ssznggte.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ivpasftd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dttdaxvx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sgytkxyc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2yzmfpvew.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vnbgohmv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ihidwves.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rocgukho.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zezvqofm.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2pphsawwf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2spbtgavr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jfodhzeo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2kigpqanu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gcuirssc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mmuocbyh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2kycyrdre.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2qkewvukl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ejawjkty.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ufdwwnqn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2wgbpnsve.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2dgrzehvu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nyhxqybn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ncculfbo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ouloliuf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2pnqzzfkf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qwjbpuna.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zeezsiqa.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iumjoefj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2yifojbxq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jactgpiq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2udkhoeih.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fscvuqif.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zxbtbcrm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2kikbxoom.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2lnymqkwr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2lvbslsts.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xelpsuxn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2nbfwqkdy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2drhkedce.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dhcktlhg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2odlegxpv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2twvpsmwv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2myoplggd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2gkujeaqa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2radayegj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2yuoqxmto.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2scojcinz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wrgtkrey.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2mlrnopcs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2dyghilag.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kdeodody.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oqjvufbw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bruzsyhy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2zfvvuvgf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2fmlmeqkg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2vexushhu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2nxmsxjja.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2lpgcrvgc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2fctfswuu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2gnionlsc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2fvdpjthm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ejpgxzxb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2wzubntxs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pkyqrqrd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ulwpvreu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2xbvnglav.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2jsbitpuh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2haickrhp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hhzucrwg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2jmwcutbz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2xxxyaxkp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2vmmgmivn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2kvuibawd.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2weybkcev.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2flvzomct.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lmexmzxl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cqgznlgb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xxrrgwbo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2jtunisku.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2rruczwtx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2cowsbhrd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2vwgxyyzr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2orvgssfm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wrzcghsj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qlebjugu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dztybapk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cdglsscu.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2heseaayb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dzvmyqah.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2agvstlil.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2amcouzcb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2jglguxtr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hsoyoiiw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2zvonufhe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ddqvpiuu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2vkbocrxf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sybcfqbh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2yyayjxdo.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2evhfrqrg.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yheuvufo.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2hqopskgq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2prsubxpo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2rlumtfog.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uxgbexrh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2spxkazsf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2oevgzkcp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bqvflfyv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2iefgcemm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2aaomoymd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2utyuooot.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ngbfrwvm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dfpoxygy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2jpvtkdvp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wanrokak.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xgukhnno.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ktmmaawz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ayerabqd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2wfutaobi.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2wsuvdarc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2rvuzndmt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2lqseoqpn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2weacmwuf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2eajolwci.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ttwcwmtq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2eyubenjp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2isbykipc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2pufnfaxs.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2enzqhrgn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2bxpknxem.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2brkigatx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wfbbrpel.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mthccqxj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ftflxxwd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ldqjqlhn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2crkryzjh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2nojtjjdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pizidzvn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2pcztqtmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mcapznay.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fkytmhee.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2hkopkfjl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2wdcbmnnr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2numwevjj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xvzrqmnm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2jcwgsccz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2mzcwfscq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2uhprlzmn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tyrurvce.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2fakwcftj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ogdoqrak.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iqrkzlor.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yytjprfr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jfldptuw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hgegwbuq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ssfkqxep.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2osidrasn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2uvnpozgr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2anspfzqd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2mgcsuqsy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ldsbuwgu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gfybwdjm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fpgqewgm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2eyeogqkf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zlmfkgmq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2qvzkverx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cqiesmjz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2fqmyflnr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2engdzvrx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2lwcngqyr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2bqygxlwk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2plwswzwt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vptrysze.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2uulxhsuv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dextieim.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2krmrghsv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2alkyvvvg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2gdexpykg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2wqvmlwmn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2czkipidh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2chkoamxt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ggkmzzgr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2tntydihl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2anpkqyqq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wtjzqeyb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2khmwuefa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oudzbduv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tpkixgoi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lovtyxkz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qyjzmysb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zevvpooq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ctgxjfqr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jmmbdxcf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qezziizy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2harydbsu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2sdilfszz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pzeavvqb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2kziffieo.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2isdohgah.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2dlwbhvio.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2eyciawot.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ledauwbm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ghuzeytj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2iaoyodfy.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2nrlbjiav.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2lgbfokpe.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2trnnjbij.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ndwlotop.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ffrlncjz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2yygggwwj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uqilgtdk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hjmnxhic.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2lmlbkqlo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2sgazixzl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2cqyxzqib.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2inbdsrap.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tenrvpil.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wnradvdp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2rvhtajny.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pmvxhnwg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vnvblvhd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2vcgegxjs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2slevhhju.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2xblqgqrg.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2enabnirz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2piychzin.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xjjjzrzv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lodyapui.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rdyvztig.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2gyzrzebh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2sgoswoge.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vprcnxuj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wywgvoxj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uovcjhhm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mefrixuc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ylokdgqs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rjsmwhxq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mofoxwem.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2oxldhmre.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ooyljjza.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cevtavwn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2cuzubseg.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ofmgztdv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bhsjsrei.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2wcjwdaux.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2thxqebuv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2clqowkwu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2pqotjcjy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lpryjdzz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2gmdcjotq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2swxyzedy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfwcwyaw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2oihkcumy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ivixrmib.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2cwnctgwg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2jgqnfcjv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgxeqirh.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2jazionwm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2bngqjjit.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2vkfixizp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2rutkiayu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2axusiwve.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ccgduydo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2symbbbhb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2jkncpynz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rsfpddrp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2osthcfvr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2vtiwcsno.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2oysnmwen.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2khpisolq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aqwmykin.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2vtehaalv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2guvotxab.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxltfncz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rblimkoj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2uzdyeriy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2wccxjgmq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ufkbbtrf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2rbmqatwh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hnuaufll.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2pzfvdosv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2tbibqhrq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jkwggvej.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2gjfkainw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2uelhhnej.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2qeqatxkc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2oyejrnaa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2skkpcciv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pwvausqo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2quilrovu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2uvfsuqzj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2lgnuxiaj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2elrmridr.html


<!-- 参考信息 -->