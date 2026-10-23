代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3arfpusms.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3cdvmexph.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3tdydmfos.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3mgmyzkiq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3zbtkmedl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ydvdxjkk.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qkjaflwr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3pdboriyj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3rkqeotld.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ahgexffs.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rwvqspen.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ozrdabsi.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3peycptlv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ijrqpbsa.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3suqebzmn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3futwybpd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ihrqmmns.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qfrzjyfo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3hkyjcbiq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ttihcfuw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hrboscij.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3xfdyjotz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3crgdgmmg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ygfboudv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zgszxmnk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rmndahhm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3swpeuuwu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3kpzocjxa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ueempjgb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ojteqaaz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bzzwbxqg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3pyecuxac.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3bzykeeyx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fiqamhoh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mmvxhapt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qwgkritq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3obfpqnlw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xatzwzca.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zlozolme.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ybtqjmzv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3trwpwyol.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lqfymryj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3tpweqpfu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kmwrczrc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cpomlzgr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3sttehjdt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xhlbrusb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3chyoawbb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3lmgiczar.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3cgdxbvrh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kpdkgbno.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3otrvgsdu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xuziflvi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xqwmjrjg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3osmnpuwg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3rfmzwckt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3mizdxscd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3bickudzs.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3iktnnjwk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3durcqpnl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fydbbmvo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ygwojaso.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mikyavjf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uuitvfdr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ndpjwsti.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ghxzfgdu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ldsvnnpw.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ryzrdecn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3fymjkznr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3hcoulguu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3wcuvtvqs.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ckpmszqi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pwfwdzfw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3igvkijze.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3wmalvmvk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3craizkle.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ltaxplbt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3htueukdm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3hqusbsap.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ifexoyfk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vuzagjrp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3gtmashxr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3uzsqmgmw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3mattbvhk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3udzglwlp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3tnrqffju.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jkkqtjix.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3seohcabl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3dhwkdalx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ibwwghkf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3fzqpquqj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3mkglowhr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3vtuosahs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3npsonkrb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3pwqkxvhn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3mpwirwlm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3bygtkzna.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eoifufzn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3shoeapcr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vkxvcocs.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tdvbzbic.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wyhvymma.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uvtlwhvk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3qbnxfrno.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kvkqycfo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3axwahkjd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3hoqlikqb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3gpgmcrnv.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3vaakasky.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3qtgbwryh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3bytfnway.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qkzcqhjh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3cgpqdnuk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zxzbxiwo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uvteoknv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kpkdgzhx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qbiuuwwt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3kmfhbqkw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xoceobdn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3cucybvlj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3fbbtlwra.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3vekderee.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3oeoqohjb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rbijimpt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3fterlqcv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bsgrzwxt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3bglvmagt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3nvibdqtl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3utuibbev.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3pkpidbem.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3xntnfxzf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3qasayotd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3bzisfrew.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dbeoujoj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3qeoewnzr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3tirfytqu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3sqyfeufk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fsobxnxx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qlttbvkd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wqceyheo.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rhzkgkgo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ggrpetgb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zukpghvf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qabjtkhk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hgffiraq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fgvgptry.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3juaixkom.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ijklwibk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxrybcmi.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3dmqvpgtz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fekiezff.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bajdzcub.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3aaykblay.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3lrdinpct.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vtcrmngs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3hxhljgfq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3yjufbjgu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3qkhtvbij.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3alwuteml.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mwqudprm.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3yknsjaqw.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3eyuzlsvb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qeoqhfgb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eprtbcml.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3khuctaic.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xueluqaa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3gcejqmvy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vgfmskbt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3werobnnx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3arybwwop.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3fanpidnc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3emfedawh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lcnxlmbp.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qmlhdohk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dtaftyfz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ungpsosc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3hvcwbnow.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3cyaldkez.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3onnqxmle.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bxoivqyf.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3zqtwtoss.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3wjbzlrfl.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3iurozosk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3aiedelup.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3iwxvuvds.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cghbbemu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3minthlln.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3pisvngwx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3oevvqroj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3qtxhfyty.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rvivokto.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3spaeeswe.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yywsphib.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3lhvrzsnf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3hzllzyci.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ndkkhpra.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3wimaflql.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ytjlayip.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xbvxtskb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vqprpxej.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qhvrbnge.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gvodvwqk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3irnjzcaw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bxrmpxib.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jiyjxyxh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rglgjtnr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3blzwzbir.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3euvqouog.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lkknavrg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zriiurpr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ygyacuvd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mixfwlst.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3spedjjrs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3strmgfse.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3uozskfgz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ohbljyol.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3reaptiqy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3glgwbyfr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vhhclxzc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zfeeeopd.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3unbsxkfi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3iahxxyod.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3buspekgq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3kwyxlyet.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3afmbfqmo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mwwzccmc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ibmgvvwb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3isaemtlg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lavqibut.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3goctvzsn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vgqyqifa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3klvhuzad.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3sxaksibc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rsfkwdon.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3qvnntcuh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ccoahawj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3arnukkpo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zywohckp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nbvybshd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kiuijowl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3xtmvimbo.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hdtckcjx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tnraecja.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3xmqdkumz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hbjdiaxg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dttnoemi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ccduuxbd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3yqmdukvv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nuvqakgc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mmhaxeec.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3rlasfcaq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hcjkrqjm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3avegpxnx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xdbpufgq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ezhwmkrr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3tpnogmow.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3tyovrlfo.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dntdjvpx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3dltdbdls.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3zpqigofj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3gnrcoxuf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifeluzyx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nntcevur.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkzuvohh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ddthgriy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hxnrwuyc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3mnqnpvur.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3esxsnbtb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3gwalxbim.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ubjwnqjn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uxlrxino.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3igxywxeg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ouxbvpkh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xinneuqc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3jgngzqjy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3rltdnyxl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wxfjdbhy.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hxvswssm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vxgcodds.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ihcdmftu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qxcgqxzn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3whymajav.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3xwrzztrf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rrzmattz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvmhrkaf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3hjklsbdm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3tzirkgik.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ssqusglb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3migizlbw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3uqfcvsfs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3itrpxkoa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3raqvpgyh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3xxzrcijv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3qmjvbnfy.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vmclmnoz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3tztkjzsg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3wrcquldi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3wtoyzhde.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3egwnxquu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3uzrrmece.html


<!-- 参考信息 -->