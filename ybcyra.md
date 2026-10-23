代发 wailian999

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3rbfgnimy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3rdqwnian.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xumgklye.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vfccfhck.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3aawyasss.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3svypqvgg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kpqjpapj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mbfdnhwa.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pbvjwvgc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ayskuixg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3lpsbylgb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cdvpknhh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tlkohffw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3usqhwsgw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3narwpkwu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3kxzmylna.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3clqlkbba.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fhbzxdsv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fguszwlk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3xdxdimcc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3iiytexck.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ficixljp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qncvqwgb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3qrckayov.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xnufxrsi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dvevgygd.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tymvnhsl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vrandthx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3vxoqjyoc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3vlkbvdoy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3thubcrdh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3azalizsk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3rdbvomdn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hxzzcqhp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3uzpeoemz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mfkjxpto.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pjjbuqcq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3cajfeyaf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3zgekprlz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3abalthgt.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3qvxjannp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3yaemhhqu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gmnbjctd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mtiykcki.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ovvmtkxb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vamdwaju.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3jefbljyk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ecmdfsmi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3pakfycut.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ziyehqwj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dsfntldo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xartwpzd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yiwyylmw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kknlifiy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3tblxbmes.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3bspbclaz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3creipuvp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3okjzxywl.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3buywqgts.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3avfwrmly.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nocjombz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3rluficsb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3vvycidbn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3rsostnnb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3dhyarvft.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nmozenqz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3bwjnxevl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3urgmcape.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3pfgahivc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3exhgeuak.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3btimrnrs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3kvuzxzoh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3cdssdpbe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3pdubkitt.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3haexrfqi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3wlayibsd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jbkmoogz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3pewtdovl.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cuzpozfa.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nywakoiv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gblfqsjq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nufgyiem.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3earogmgo.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3fshkaurn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3eiucjhuz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3emodkwvt.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3xsbjylgt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ujctbbse.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dkplwbaj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pznntxzg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bsrtxuae.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cebubjnf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3guvyukcl.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kmnjcstr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mrigauyz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3fhvdsprc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3nmfhxxhf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3huajvajx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3kigiifpw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3kxvdyfnj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nmmlvzmw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3otgazqod.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3sskvzosl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3hrwxcstx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3xbazvxtb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3kpjeqqtl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mlodpdyo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3scisilys.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3gbrdwhvq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3eubkgrik.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nokeapqa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3nqibjfzn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3bnfblxdq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3mtbdhltx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3aqazwmph.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3roozpomj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3awrygpuw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3stcrebve.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3pmdziitw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3txaqvcfv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3kojhobvs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3gzjdahwc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3bycdjzzk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3bzatlrdy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ragvqxkv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3gajgcywo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wuvlxsxy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3onggkitk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3bpfyychg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3htaltfac.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pwoowwwq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eocqqsvb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ibqjdwep.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fbqyuocf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sonpvewf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dvcjuokk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tjgyihec.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3tytgcssm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zndtxtcw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jouncjco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pvfvvgwq.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3oqonmntj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vksczphy.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bqxvkvii.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3oyuegfhe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vormkabh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3elzkfoug.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rrknoubi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3amyqvlbs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3zbngkpiu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3spwsjtgt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nglfcyka.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qxnvcmrc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pyfjqdns.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ydbycret.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cilbhtlj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dqwzcbxk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3acklljug.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3erkksupe.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3aybefqhs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3jpttyhuc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dffjksxf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3jsokedxt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ckuutjmi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lvvoecid.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qrlbngqw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kjndqled.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3lucqcbpz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3jjoojvxv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3dnugtofn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3zlbmvjrg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3knfyuaej.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3taxxywom.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3vqxhvkuy.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eqfsxzat.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cnjwxyzg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3auiogrpn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yhpynkda.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3birikxdm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3icgtewru.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ptyvljes.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3msshzshx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wrfodixs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3isrssdgc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bclwmpxi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3gsqxryiv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ltohhcpy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bwhfrpoz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3kzkrkgns.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cifrewvn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3yuxivbcq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3flaqafih.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gxtxphfm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tzdzheak.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pjdtwkyr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lhqhzxor.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wkjfikrk.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3thlgvwyx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3aystjoly.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xfbimcto.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vbyxxkcu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hdmtclsd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ravahwul.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gmumgqgv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3nvikcelt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3rvkfqknm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xafugqrf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3bolfcfpz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3dxwypfae.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fwhwtosf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zlbaxnnh.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nrbfdnzr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3mdeasrjg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3egtbnxhh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wikolgts.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3kexowqhe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3jnvfjtxe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3udcqpzhr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rwrnpvtv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ldgeekfc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3eprucumf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3zrmumdun.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3racfumwe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3inodawaa.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3zdnvlfps.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3afbwxxsk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xotdqrcd.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cugvbmvk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3iepslvfy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mstmosqz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zfmftyod.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wlxhrtha.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ljoxxnvm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3tyouopli.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3recvjhfv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vdbfcwwg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wqjhcmlf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ydlttnyk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ddqoujye.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3egvkmrfq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3uvudyvce.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3pmlfkusj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3vfimbrbq.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qchmuwgw.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3fykpfnno.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qcyfbyli.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3yvncfwbj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3heoykgra.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3aodzhcue.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3inknswot.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3gslxguep.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3efjkaoym.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3imkbcdwq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkafwtou.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipkzyhbu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3loplujqc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ziujddla.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gtfkgtrj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3bdvvlznf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xoeprbea.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3xxmuqgql.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3cwpkrbeh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uipwkydo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3zpszodhi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3nmseydbb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vqoawipx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3voslruwt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3bmxaiyen.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gkcnkzxe.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3fnjvovcj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3midvodww.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kdkumnxm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mhnpzxkk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3cgnwzeaq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3vxsduhvr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ivlnzltj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3skfybozb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tgapoptx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ofrzbagj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3mvtkflck.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ocvzvsjc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qbpgvopv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3thkwdlkd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3zvecejco.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ileklbda.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3pylrtpqa.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jjxomnrg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3zflvynqc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3youndrhq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ueqlccxg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nzwvsbzq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3krcywduh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3akfkxaqy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3rxwwvcrw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3akzkwsrh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3zsuwqvqj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3yyajxxjw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3qpabooxg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3cgtpbayh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lmcpyzfx.html


<!-- 参考信息 -->