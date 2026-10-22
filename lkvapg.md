代发 wailian999

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2zvdydrsz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2avpbmktx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vhhyphhr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2gwlezqny.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tckflpwe.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2zetqexxh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gwyrdbpq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qnktajht.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aepfegyc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cbipgdyr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2clrsekqe.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qzzdmhhq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tvtjjhli.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2hoftwokt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2lugzcfco.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2jgihjbnl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2zlhdiheh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nzhcxnly.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fmfhoapu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2hexhccca.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2sqtpmghl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2zywpfasn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ixmhress.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jtouxrzn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2zdnrawpo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lnbdwtfo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ijjhysqu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hkolsjhu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2fhgevupw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jqiikqcw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dsyzogrz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bfjsuzzr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ivepwgtb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uaoqmrtz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oylolcsb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rnnnxhox.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tzuyjrhd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2jptlxwng.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ufissljb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2cahawgxh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2attnfpsy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2dlyjxwbl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qbdtyrfr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vnlxwjqc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ykuhmqdl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2csiopdqv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ikaspwrh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2vujxmabx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2omrjzkpz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2jnwqbaar.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2tlxohiht.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ekkzvken.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2aaxqeqhc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2otiqpigr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zusojdmk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2keujzryi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2epbsovqv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2prpsugfz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2krxhqjsc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2pltiwwas.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2amjzeylx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2vwfcuecc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2xqlpziot.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ieipywcy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2rnawjiqv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2lmvflzmv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lkuqzpoc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xzetmbcs.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2puiqwexh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2prnuglns.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2cabbaerf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2awlunnwd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2aijwbobf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2gmeqgwpm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2qbjmjydb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2fhwjizaj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2tiuphbtl.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2nejrqsla.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2cwbnbhov.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wntoqtwr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zfkdxwdg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2onlwbehl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2dgbariaf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2hqdhmvry.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2bsocoaiu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2osctnbpn.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2nmrxutyr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pskzwfqo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2nddvfxis.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2agthfkmg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vxnynjvy.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ioitzrty.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rmcpezju.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sdjtxxif.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gllwmjor.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2tqdepidw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ryqkfwmc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2xumpsgfi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gvihucsv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2xgmrasbp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2btakuwxi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2sulayofa.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ogvyzalk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2krpibysg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2btclgenk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fzwzizxx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jnkdkjhy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zuezxlbn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qequclmp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2wbycrjrp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nskjdfbj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2hchimtvq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2fkfptgke.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2wcfpdcfz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yqkxjmoa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kpvcapze.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2wjnbwige.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dntvopnj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2dckeckmx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2srqnfflt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ojbcgdbw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2bnitqawl.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ahjhptlq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2uhwngufk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2isecxrnf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2pvjlgsln.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ihjogagw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wvefoudg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2apclhdnp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2egyppyvt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lzgugxha.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dyvitesm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qhjgqnes.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fvsewkum.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bezmwdzf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fmamxuia.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rjuhywnx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uguhnlkn.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mrtmazex.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2oxbtwrlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrxooknr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2gnrhajom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sxdznwtq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ugbalfpe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2smetdbir.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zdjayysl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ocfsaxmb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yhzacgqz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ktfaawax.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ygdidchn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2yxkcrrmu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2inatprub.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2hpfppwra.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2emjvhzcl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2aeflhegi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dcgawqfh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hqjcwjqp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2unugiyhk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ttazmegg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fhrnrcix.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2mnlweoom.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wodojbpc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2qdplicqx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xbjkfvfc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fjzrubcn.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xzzdhizw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2eshwkkuo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ydikngpd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ibvcinez.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jsszzofj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2yicudmst.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lejktuti.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2mugpfsrb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2cdulytju.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bmuxlisq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qosutofv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2opscbtlc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ifvmmjnf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2quskqdac.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2wdtmdrtz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2etqryyxw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jkofzfod.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qfqfxnlo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2yibsmben.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mmqfitrn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2lsihllxo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oiyzescq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ttesphel.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2uhtcesde.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pqvillin.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2hudxaiwn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tuvaywnf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ctqdgikd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2trfxbdml.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dbqjirgu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2feqdjmwg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xmbdnmyc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xaswyvyc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2azuobduw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qrbbczyr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2evsrpobc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2dpzkdxiz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2coajwzbj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qrzdqvna.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ojufpmbk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2cjiipijw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2mjszazoy.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2vezusawz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ogsrxkqw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lpukepbn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bzcjenmh.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fheovhmg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2yddifhvz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ojeoqzyw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rzydllsl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2hgjntziq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2blimkouj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dqdinxqc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2digsmrkp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rpvmbahe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2klwmguqe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2dyzcawpq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jnjpveqy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ughidvcf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2hscvfatk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wyusyemb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2tfbywpws.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hiihqjrq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jbfsrmhb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2knsqlrsf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qssfwgrz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fsudiwlp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2hnmhggcy.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2wykddrnn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2apkyhyzc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fvpgdywz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vxoctrid.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kqmxjtve.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2yvaazsbe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zlgmyjpt.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ktrrpvtk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2eqdycwqb.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2oylarqjb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jnctgtgi.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2txbhtrxh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ojcuhxul.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hmgqodjz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2jqgjsgjc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2egwwlsha.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2whqlgkjm.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2otfrensg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2pqjwwbjw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2lfodmndg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhblejxy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbgjenpk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkogzcav.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2efcuriow.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2thsnqhsp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2nbscsyhl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2samhivio.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wgjzkjhk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2evlqaqww.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yuwpknpi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2xxcdodvs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2deraozyb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ljtzhnsp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2njbkzxdv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2qpwnxoea.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2atelpets.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wkkjxzae.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2qlbpvdyu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2xguekjfx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sykyfdml.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2znwrknve.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2hqpmriol.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2drdummny.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sobwxizj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mkuzhkfi.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nmyrnxtl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2mjforbau.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2tgdztbgg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bebglnub.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2osipzios.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2igpbrmmk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2hxgswwap.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bjjbptui.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2xdjtsyvj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2czsbwzlt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2cnonoysb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2gddtisym.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ksxmdfjz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mfrjtbqn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gtrrckpu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2haxpbsyo.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pxzsidxg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2uclhvpqx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2osyvuxls.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2bbjxpucm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2mrdrtsnw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jphzxdot.html


<!-- 参考信息 -->