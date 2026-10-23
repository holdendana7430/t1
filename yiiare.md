代发 wailian999

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ycrzmhue.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3zawamrvn.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ccjqadog.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3fqaoknes.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3rmbtvsfj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gxdyxxuo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dachmvml.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3idxftcfb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3llykmuig.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3tzjltsgn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3szvvjtyv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yfbvschc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uxqxiyvf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jdacljgq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3cdtoneqh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwvonosy.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3htqounxi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3pxsjvatm.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3cuwomglb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qklpwqjn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3hzvbknxp.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tvryqiie.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hekmfdfb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jamgxxrx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3uuiieiii.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3nioarnat.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3illlbezu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3stwshlxe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eoovycfg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wqtuldeb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dvbanmkz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jlkoaizl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3wmidmonv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gywxdlvy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cqvpqkxj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qhcgibsh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3owmrglti.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3leugaqut.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dqgznexa.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kguflzeq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bjpguxfr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3xmxidysq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3fcqutadj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3hbyshdxx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3juklwity.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3tahnxrhu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3efuzrrfh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ldtkvnfr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kdmrvaeq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gigmjwqi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3hyhkxvtk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3jqobmieu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3icdkoziz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3rwwtokfk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3yrqpakyl.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nqowtukz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pmpcujsl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3vmfmxrpg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3batcjhqw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3kdwdgaty.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mezkkvfo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3acjaosnb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3oqfmldhy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3bbrotibm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3kpbldcab.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ixjxhkjf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3rqmajpdj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ebsbridd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ajtfmnui.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qudwixxr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3sbzqitgv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gdveltxi.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3vlrjkdrj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ntdfovwn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3jturnroy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3chaofqhg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lvrnndqr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3anyvtjpe.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3gxnrafbb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3huwekkjo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3vfravljo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mmsuftjz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3enxczvow.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3zxthcfye.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vijmeinv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vegszsqq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3wpdlhnwz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3lgwkzkbe.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3pbihpsvd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3kbclfejl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3zrekdbwp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ldkcouuw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3eftampjd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hntntibn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3owradsqz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tlpczzmb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zdravski.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jzxokvrx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bpuvzvyh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3xmvfhbut.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hcrgzopa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3rywidqsl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xfvqzjgp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qczvyxow.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3avrihcbw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3durgyekp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ivzspqyx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3qcmmbqgh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ztoynzla.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3nbuuqbxe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3xopgeypg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3whvzwqfx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vnoxkpsh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3nftxicep.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ftvznclb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3wngijipq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3oocpyljt.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ujtyhajr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xpcmcmgw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3temrfura.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3mfgccada.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cbfwlgfo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3svwicfnr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3ieumrnls.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3jdjqelrm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ocdldswt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3votypgcy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3oifwdmsp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3sknzvabx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3esiicjbc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3zwxfzmcv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3aatnsrks.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gjkkycbi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3epzptidc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jonobfsg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3qbpozoqg.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rjtqomzn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fgayygbc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pozstcpe.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3omkehbhn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dckqamum.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3uevkndiu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xsaeqraf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3nuffspmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abudrqad.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3znoooqfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrvexbzo.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pxsvdupx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ptoxzzfw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3fuxqykoc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3nwykaylm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qslijxrv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3picimrok.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3kjpjyjkp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3dclhdkpm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bdukftab.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cpwlvuoy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3buqkmesw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ibqyoegx.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3uirsieoj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wpoiuvqu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3popwqkqt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kghemxlt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pzithhhc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3folqebjq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ljhkuoot.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3vfxiaehj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hlvyuaun.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mpyrdsoc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3exvejnyp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3glepojmd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qfsotove.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3wyswhkgn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iakvmhns.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3pqoixjsj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xcidyjug.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3hmomtknx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3sngarrks.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tnxeaeqe.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hdqbryph.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3amtofucv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vnzemitn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vgledpjq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3xvkflbit.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ulsbvens.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3eussnrjm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jbmbcsba.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ithbprff.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yozcrfrp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3fcjkigby.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bouruvpv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lfmzqnhb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3drnronfv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fbtmuhwn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uquzgfqm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gmvamlvd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jpcrctng.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rxqlxruz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3rxotiqrx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vwthhgkz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dnqghujf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xgodeock.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3kscloeae.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pnngsmjr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rnzgrjyr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3mwktidlo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3vtzdlnqs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tzoqpnvz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3noesemnr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3poeextcl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3gywshqgs.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3gotytuvk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3basnfzep.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zzfewhcx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3npdghtmt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3knbshlqi.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3mjgrpcol.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nxjtsmsi.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wvsoaima.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3rppythuf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3urumxgnt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hmbnahgp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lgzrjqlz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ejzlvahi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ibpkfyfv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3bpjltyvu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3rfbpoodw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3sltrdynl.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3blucdjfl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3avsbrmsa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3pwjrikll.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hksvzstt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3quxflehw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3intipyxn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3staoselj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cxvoxusx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3letfsghm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3aawjaaqx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gvyuiytb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3eflabcsp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xxxvrepb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zutrurrp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hybdaovo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3yxfhejxz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mpcfydgv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3itofrmcr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3nsjaasqw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qqmhklst.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3gkzfqxzc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ueupexzr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3tnqgctkl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3rgubhjke.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3potdfspa.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lhtizfzg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3kabnrqtb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lahpmlqs.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3huhppbar.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3iuxafhay.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yncoeqyq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jyqyzlza.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3edkynlht.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hjgrapsj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3girbbiif.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujalbkqh.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3fkftwrtv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3xjsswfuf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3nzpxalwi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3vwpgzeoo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3khetseeo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lcgnrjun.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3vpnfykof.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3czloraxv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3spczzbpr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3wwbsvfpf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zmpamtjw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3vmuaccqb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3eojfwvyv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3fjlfuljp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3zttyrnyz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hznronuz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3dtrjywqp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3fmqywgmm.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qzklbnzv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ntgaakwz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3zthoalpk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ofkfkriz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3erjhoell.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3npyufqcc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3tmfdzhux.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3tjnralan.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3htchbkhg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3aqbjxaja.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3noezuzbp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nweteten.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3luelijxj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3etqvvyiv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3aulyypld.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3xtexustx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3oebnfrfz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3lysqucbm.html


<!-- 参考信息 -->