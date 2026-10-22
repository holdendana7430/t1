代发 wailian999

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mjijoyze.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2lxajojnj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eeinfzyu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2qdmexyjq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2hkxfshsy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2qifbdwjm.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lojkgxoy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2fkibqnmj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2dyfoxbww.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2inlnpqzn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ynjcddhi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rxilygya.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2joakbflm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dumzbkjy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2maeplmel.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cplfsfky.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ndupejyw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2qhywptkq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2piiprmxx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2thrahkgn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fuaqazow.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2furjazvb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jpkfpull.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2mrrvhadn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2iofbrdua.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2yffbkuca.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vfvqcyah.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ytcxgnla.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2gukcfivs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2efubgkcl.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2acaekbsv.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zggeyxbx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2barkgzcd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2gbedcaxa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sohadeis.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2khzgtcta.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lvxsfsec.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zwliqflb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nyckfgze.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bnvofedj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kkmorkkz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2uttytztv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2sfisvwqp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2youcroxr.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2nfndhvqz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2wneycfjj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ktzdtphc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nxffhugb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hsptcxcl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2tghtmbsq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2wxsuenis.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2wptaqrvg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ubxgclhl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2acxtykzp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2kgjklhhe.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tuazdheg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ftigrddf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2lmwlsxzz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zavndeyi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wsywoatx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jzauttib.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2hhevfljc.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2uxobmosz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ugwgpppd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2atrneyeq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2zfeyjxwe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2smxeibty.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2cielvime.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zzqivljr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ijgsqsaz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2todiwrkn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kgpeggeg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2uxjzfeud.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lcwslldy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2erpvasyu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2riqbpkrt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wyafngjn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ntqtdhhn.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2neculmwy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2sofayynu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2jsqmtanu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ddtdjndf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dwxgkmpz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2zkknlmgl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mekmeoyv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ikiwmuek.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2lvppjkkl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2eblyeedz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2oowojtmj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2uzzwyeau.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2tpgwvhux.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2viqrdomt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2nwgzjjyt.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tdjyvoyh.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pqjnenrz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gdomegpf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fmumghlq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2icwtlhld.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jonnczip.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2iouvapsj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2hvmhitqh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2wuxaewdg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2diqvzgwg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2rqqnjbms.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2lxqrecdu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2azxovupr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2qjxvhknq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gvbygsax.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2wtwbfyde.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ixjijjbp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mdkmdtrw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xhgcbpsc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rzlcxhvd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2pvowjdeb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2yrrlvcye.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2spxhjvxr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2fpvfycaz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2skcgksdq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2jcfqyshs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ciwbpbme.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ucxjagju.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xxzmutob.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qhtrsuzq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2pnjskxul.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wcxzukll.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2zvowcmvp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ehquwbsu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2gopnlbjz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2mzeczhjv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bcseozqg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2tikxrhqd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2btnmurpy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2axistxrd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2godfmxlw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mlvktmea.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2zmbwilqc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2lmdocoeo.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fqljhkpi.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yahixqsl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ytuljadq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tilnfhmq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rtsvlwaw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fqdzmvtb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hwbyyuuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvxiuvao.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2gaproozt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uywlsnzx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pdfyjpvh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2vttattml.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2kdjrdnix.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gqhvyvik.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2smtfzgxc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ymltswpk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2odxmrdpj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2mhmtyfau.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nxiesmjc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2dkdazpgs.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ehoecptv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2qxdxulww.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tklvbhzt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xjmblumo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lpqvoshr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2aaffrshj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hpxgospb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ejixevzd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2evquluob.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2qtnuekmx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2enaumkmr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jgebppos.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xmurhizs.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2utdkkkea.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gjnehfdr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2yhbknnph.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lvzudkti.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2lxjtrirh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uqgyzoqm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2rwoddzfr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2mcehtgmg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lpnqwogo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2chozoahj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2nxgawyhe.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mmpzmhbk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2edgmmbrj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2vcgzxzej.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vkgkkgdg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2mmrgwloj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2znuoaqyo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oifgukad.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tftwioay.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2syditsqc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bfzltwgq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qowjvntl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2xeoedpjp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mdvflxif.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2haufcrug.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cildjftm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nuiiqkwx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bxfokkxz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wvscrgiv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2svheignr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jknbhoqk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2indyrjwd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2civksffi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pvsmdqbb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wpmfqgla.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2vgzzmfnn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2pwqkndzl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wwxaarrp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2lrphzren.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ffrtjeet.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2hwaglhag.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2xzpqarzh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2sixfukkd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bmswazdc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jqlqkent.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wtzyyzzn.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2cxdghpzx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ehxsklxv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2trilviof.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2tyijvqub.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2oiwqfpyk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ikupecqx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ipmxjmyw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2udhhwpsi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2fcgfhhjo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2coctdshn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2lilqzgju.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ivkevvxd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2fhiimujt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2csmplcii.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2wrbkisja.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jqlzrovf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dcpfjnjs.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tpgfmapd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yqftrccc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ghpigiui.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2hsgftopd.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2awwswfuk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nowerklm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wvtbfhff.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fgfmmfqn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xsixdifq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2sggnljrp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2mhapsdim.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tsvmkqma.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2psvsbznh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kuzdcgke.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wicugiek.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2tohkwlvn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xwxphuut.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2socjasqh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2cobisixb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2vouahegf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2evbrelki.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2aazktphv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gdverwfk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ijyvbfat.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2hzicvoym.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cafaubok.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhjjhith.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnbvowbk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2usvdqzud.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2uiavzjgj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nppimrhb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2hyufhkhq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2jnzxqkbi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2nvnhpaqx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2mduedzju.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2solgzudp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kszcpwez.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2bxvbniwh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2uyutqfdj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2uimzqoug.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2aiizhshn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mdemiskh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2idnqbubf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2bxkpjxfv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yjebzxyv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ihfqgxrp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ksdnkpal.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2yoahshgq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ujxdryfc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2qsfclkom.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dvrdjdvf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2aerahaux.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wkixmrsb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2prabgiws.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ecoxazic.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2kllaqkwy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2pqlimvog.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2axrpjxrh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2lrosprxe.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jrmhkqah.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2gzdmhewf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zavnkmdz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lwjpthhx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2tanafcsu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2bghctcpd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2uotkvzwm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2trurauwf.html


<!-- 参考信息 -->