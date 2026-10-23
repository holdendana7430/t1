代发 wailian999

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3soxsouji.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3splhvtaq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3xcdcqgym.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3nqgbkbzd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3uaznimtv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3nsecqvbq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ttrokfzf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cypabxdu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zdlaerfq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vvfeiagi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3oewtxfqd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ocjfpfbv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3kchojhlb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ghxmmiph.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3qixytfpc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fzgyndwo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3gnflydcp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rzolkgkr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bawxkqqj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bfraqisj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3kbhfqykq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3axieygoa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3izvzmayk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3sluzcpnd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wvfgwyff.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ojxddnox.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zfadsknz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mpmkwdmi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3xflqkzwl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3fvxppgvj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3csnaqfiv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vedktkrm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3wmpedftv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qyumcgqd.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3dnhihipw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3adlgckvf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fbgjnxgu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3dscgzano.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3lzuqshja.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3fhsuzwcv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3szdsnecg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ejbdsmcb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iasmjqti.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zssftnui.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pbzmazbr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3usoasmjw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3sewpqebr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3untrirze.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3vuyhxmxl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3bmqkavtc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3naljrsiw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3cmrbqhqk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3raxtslag.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ougieiie.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lfybmrgy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3gageuewy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gunntdhz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3nkaxbxte.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3hcvgmidv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3nlmothsh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3bwqkpkon.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3vlhmsdha.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mfwgrtuz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3epghdvgf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nsheveko.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3znmydlup.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3gdvqazzq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ljsgcuqs.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3jaxfyohg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3itfyphcx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3czjqahaj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3znzblfdg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3yrgmcgvx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ujcsvrkp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ostkbuil.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3skyspobb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zvrrntlu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3lyqenugf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sllzclze.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3vhufnxif.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3akqfzjuz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fcotqsdp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3mughycoo.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ruwyjjls.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3fvsrkwqf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3hsrcszrs.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ojiobtbv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3fjpgntim.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3hgnjmnky.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hjbxweqm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3blxvrhjr.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rurdzjnh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bsgqeiqd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3plmetebm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tdgxzrfn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3tzzrvyhn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aeiwbpka.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3cgbjqvqn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nhkpbpyk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3kwmitjoc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wzumpsbs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cbtwzwfh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3lyoyqcog.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ticieknw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3coijzszg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ywhbxwrw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tdgmggbq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lcztgcai.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bixlizqg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3yzuctzmw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vweceleq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3dwdrkkfc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3kwzdcfxb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3zdzujxqm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tvvbisgz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3befdnrlv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3maelbnmr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3swhqmwnx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mhnlsbdq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3nfzxldzs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3nhoxdazz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3lksqrjnw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3urwevlaw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3jwexgakp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vhnswvdu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ahbkzree.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ltxeulvj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3finytuog.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3sfpomsws.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fqyfbvre.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hkapdarj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dxjsynql.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zmuxdgkn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3unqhpand.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gmlhyodq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3koqbpxqg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mavjdzyg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3owctqhak.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jhisfuby.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fqbocylv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gjzauwxx.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3vqedetjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fecfbwht.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rcqwykxs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3vplleahh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3bbpjvcak.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cgdqapyz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hlvpcwbn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vdfkyfuh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qgygqfij.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3cnbpearj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nucdxyik.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3etkzonrd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xlwbkjgq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yrgmmyiy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3odvavmzc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pzqivkuc.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eficqlns.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3cxjwzfvx.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3iuzmxkvk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3slvnuinz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rmnkefkj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3vgrfdxjo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3axnxqvyr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3quyptpys.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mafvekvg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gmwrmwhz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ykgyorax.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3manibemo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ntlrelht.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3pmmfyrgq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kzyfnxrg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3mtbyfpis.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ttooazrz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3czyftabp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dehwxcek.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3mlqgsgwy.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pcagxpff.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eihuipdb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3xesizjls.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tjfjwzzp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3gzrfneda.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3linchmqb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cbyteprt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vakeqpyl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3bpbnjhcl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cdtpgkpu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xiydcxjj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3yhhbajvm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vweurvuk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ifgxhobi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kmiaoupb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hdpoxmdn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ptgfzybk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tireqhwr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hdhnhllf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3syfvchsb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3xzwmcdgk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ykrztehe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uentwwqw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3mpfnlmbt.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yekceuwe.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3bwzpgngw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3dhnmuowk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ajjssiap.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3eijbifmm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3wmfvsaja.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3vtlcnsux.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3pmthmykb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3adeddrur.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qdxpdqtd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kuihaktd.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3nzapwlcm.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cugegrfl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3skqwjtlz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3cmdnajtt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ivqxmunf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fsjdtwtb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hbhuwrdz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fawosode.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3sgrrwhpj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3hsswcsqk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hehvoiqa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jqpcijeb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ttkrekwy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ciqsykyz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3cwebfwpn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3knbvdfkx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eoooithb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cdwvcmro.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yqzojpri.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qubkhjnk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3sglxrnpm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uecylgxc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pgaookdw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ntnbutfk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uzrbudym.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vxpxczka.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3xhprdxdj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fgezktzs.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3bssosris.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3mcboszvv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qkjjfnjp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bxvqdakm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3odfxonvl.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3txbmncsv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pqgstlif.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3csxsziwo.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3pgsrducm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ydmikcyx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3wjkcsljs.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ffknappn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3dzorgtft.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3lezcfblw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kfqlrrhb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rggrhzbw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cpndrsuu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3iebejkmz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3xpzjojor.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ksggluwc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3rxcblhcj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ixyzvibq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ctocgntx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3bhkkooam.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fwioegiy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3atnspqag.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3cvpuzncv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3uwfiilnt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3oacbtyzg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3qpmhcjki.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ozotyjev.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3fkofpexi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3migzqqrn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qwmerzya.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3daqydike.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3bwzpwmkb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3spslukoa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bfjiulug.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ulykgtkl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3scsivtgk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ekmiesco.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3azdqrhzv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tfewlcgk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3pkncjsxt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3yqwsinxl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3vbteykqq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3fzahrogw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ngtclrus.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3cgneralt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3exunutoo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3owbyhnfi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gfwvjgjg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3tdxeyapx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3clizgquy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3aausrbnh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ikohaalh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3uqrtdeip.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3nceneswz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3igjjbzim.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3llvdisre.html


<!-- 参考信息 -->