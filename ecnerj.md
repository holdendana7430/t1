代发 wailian999

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3wtuqltof.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3dgapxgvr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rspmghcd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vhpjunnn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3juhygxji.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fygahlgc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3xktqrejy.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vvovqlte.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uzewoxaj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vplslkfs.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3gbcpaken.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kplqmvdk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hhnvehou.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bylwhhfx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ptxmwnan.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jehgnvdn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3upwermsg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3owaolcnm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3arepztev.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3qkojazkq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vfyiybwu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pwvcycum.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gnpdiixo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lxoukfgb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qvvccmwj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3gllehqjo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3svkbdwqo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gnugucby.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3fccshjea.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xcreevpe.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zrhuwngb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tirzpxyq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nwwcrysi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3qbixwzju.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3laabrehp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3njnmaypq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3gdevqusg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ioedraqj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rxqyosbd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3opihuxod.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rhxduigq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3tbnuwuzi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3abbnlmjq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3qeqsbauh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3yjbyblje.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3nopxuluf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qrvhxlnt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pqpiguig.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cujwcerk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dphlqspf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jvzrsbcr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3noeriwtm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3trurcazr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3elaqoncq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3sdqbvaps.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3hazbbzws.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3dnhdongp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ycnkcqsb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3xmhqmgpm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3uviwrmit.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zzlnuwsh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3uvkrxtkm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ocbupznz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3thznmdto.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3eqzbybxa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3lymtawyk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3vusvgthf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3kvcyrkzv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vlqlxzus.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ohhniydz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3rjdkomsr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3pauhwqlo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3vbgulsvt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fjflnrim.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3fxjucbgb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3sabvrnwu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pdrdlenb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rhgpfkci.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3klzvhwxw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ygpkzodx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3hmaoozfr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3saudapdm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3fgivdmei.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3mzakdtoy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3gscwcqbg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hxdkryzu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lxsyggrd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ylxfhuel.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hxmsctxa.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rbqfdrcu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dpnykmfn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ixytsoyf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3eonjfyyd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mvrvuuyu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3bqyhueyo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3govpqvlp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vrfxpsrl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3mgotmitl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3duqgfvxs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3zfmyrawb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ldajzhac.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oxlcfmfe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3boiljhpn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pminqezm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wqwdvflf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3mpvinzse.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gmofhpxo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3myoiowjx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3kxmskbwc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3cpvzhlhd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ubiyfqef.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oyghtcmb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iaglsjmi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pxpkzgxa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3fetzifmf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3atgvljlw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3riqctqek.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3iwftjfri.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3fdqpanjs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3wytrqjui.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3jtrxtbxo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wfofqqew.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3uhwnzsaq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cvynjjrg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ybdnxioj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3dffozses.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mibrceep.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cnvugblf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ayounaba.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ufbazskq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ckrsatdt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bxtsnqct.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jlvmfmvg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hpympwmc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qtotvoqx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3lxpgusjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bqwmmwvj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3zjmprwva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3guuhdxin.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pgkjkeua.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3omveiack.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3bpqzrufq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ykmmqtjr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3hlhsytum.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3hkhliquk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ntosixmi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xymxmlrf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3aygyeebm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3fgqtmgnp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3skdjhqlc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rclddhyw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ioudhxya.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jvajlhho.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3llpjgfqy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3jwsgvutz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3umrwuybw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tlfmsalq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3orjthwpr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3xhcletya.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yujfjdcf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3sroshrkl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tzqibzji.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jbejrvrs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qilfibgd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3mjbgqjrd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3txclflth.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3tvefvzbc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ootsbkwt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3reyesegd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3niigykbs.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3inqkitah.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lzlxshof.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3lvhskwlc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gwmumzns.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ekkrsswz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3mqzctwia.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ajyzkpqv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3avwjuwjj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nsqmhqjt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qajubwdk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3thqbcmjk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3jmyxecks.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ylhbijsy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hyvgixos.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3cqzkotwg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bmlcwbqa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3cwqdkfut.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3swafehpy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tqvbxqij.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kytvhgks.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3lujxwajm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dgejeyzn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3whqtlmxb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3kukgrgfu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3lkqtthnu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wnuobetk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3uafhjzqs.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wqipgzzl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3yjxegtpy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3fydkpyxz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3gfdsqbhj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ysrpemup.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3skdwupqs.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3plrmvrhu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3voyllarr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jrrppued.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ginjkrcq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3sbyznlyc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3pdhmkird.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nweervhc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lvgueckj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3suclzshf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3owvfckwr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3nioqoqbi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ukmxbdtm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vkbfuybj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cffztjfu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ozxxcsat.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vnbxlkah.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3dshopaak.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3rfkdicgw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dpclhtbr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3kqimivic.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xtgudpmx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oywbfrpl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3popikllm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wqillafa.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jhwgyxhn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3mrhwvxxn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3vmkdhmen.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wayxqemc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kshxbmzl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mpzlcjpq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wrxeqtnw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3xpqhzqjt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vhnkedzx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3abwnsnjc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rhnzrhnc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3clpaclbi.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3horyphgy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3nleqdwzn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3sivjvute.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ydgbfpsh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3vhttpeug.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3poegpyog.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lzshvsva.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3tynvskmz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qewnrcpe.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3iinknpgu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3urykknsu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppxyxfqs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfbatalu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvykvqej.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3llejfzuo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3mjwsdzvf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rtotdnki.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3lvxiwxmw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3caqnxpbu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3fxxlmdjp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3lrpgayia.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3lmsumbrr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ujgulipi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3cfwrqioa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3erktrwzx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3myufacnd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3luchnhgl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3lqqlgoko.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lirhtngt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3bpzoifkq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3eshlxmjz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3jcorokhm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3fclanmqu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iryoxajz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3rxrgckba.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hqjqeczh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3eaixsxyq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3vhrzuaag.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3nwhtudzr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3eneobouo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ofnvqdvs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3czgeyimo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qukaepzm.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3msczwhyr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3huuagcxz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3uoqfmjix.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ahstdksa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3juytkvrl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gxekztnr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3shrxpbwb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nemiltdc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ecdfnubq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3cxjjnkkw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3yoztpspx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3vxhqekaq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ecktuybq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rlgfxkad.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yhpphloc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jvkltndr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qdbwxsze.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ubjfwyme.html


<!-- 参考信息 -->