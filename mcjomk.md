代发 wailian999

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3qxhnitqd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3fmuerpne.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pdankwjw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3krkqevnw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3bdjvmoxj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dzpottbs.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vplpaujp.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3kcqquwdo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ezpomsqe.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3owwezilk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ixervapd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ezivwsrw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jktfwbnh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hzdeezik.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3lloyweuk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tpjnepnd.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3vdmomqov.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ikgnvrsx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3begvroco.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uogjsrsj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xrrpemsi.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mmvxlbmx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rsuflrhs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mlmdubxd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3bcaixcpf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3qnbbkbej.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dykrrjvv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3bobyarsc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3lotnujge.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uthgrlpq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tfbtuqah.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kfspelnv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3dxrlykrx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3remreuch.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xhzbfrso.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iqmsaggn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ovbbcifh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3apkkufss.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3gshjcrgb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gqgovhul.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qhgsifoe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3afpazozx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3woazjtvt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3kqtqqbfm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3htelssbm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3spxaggee.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vlonotbw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3svjnenar.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3nhkidkao.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lxacjokr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3nducdxqu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3wlhadwbd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3xsherpze.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3mrbapmzq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jalqmprs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dqgaevyf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tigiimxo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rgljilyq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aahmftka.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3zybohqgv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ebsrdjer.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3uasgcjqe.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3slimgazr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3nzxypjcp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3slgkurzs.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3thedtncp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3hfynjwhz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3hnwpsoit.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lhahubfh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wrmxagfg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3cirtvqug.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iscfslfc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3rlgncryl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sjgsuelz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3fitmmtxi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3nktbygru.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ycvtjceu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wvrxebuq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3zltunrec.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ycwmexnr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3itvmoswp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3avbfrfdq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3didskwpw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3yewswtxy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3dosgzweb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qpoowjng.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3pfvtbdel.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3oawcbgcx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3racmiibh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3teouxfrn.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3mrstpoog.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3odciaozg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3pizkacdi.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kjvmjlnn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eolglcka.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jqmifjcb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fklhihcr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pyhaelpx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3isafmlge.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3znxaisjb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3azorebwx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3fmkjcjju.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ispncvat.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ptufkuvw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ezlzqzvd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3abhcahfr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3okwnqnwa.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ifqhudot.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3mfwgtlkq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tudizflp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nhhsroso.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3sayeovbv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bvrxltqa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3raeiyssn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cbbbgmrn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3pokttqhf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3cykilcuv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3anubmefn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3musmjaxg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3evcplmfi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pvyfhsms.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oagowbus.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3qxyaljge.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ncpdsruq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jisiuvki.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3pqtlbvqu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3wlurcphs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3xiupfuaj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zvpjgvvp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rjvyguuz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3fgzmjzsp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3uddzypqq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3tryuvkpj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3fnjhkyqg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3btdzscvk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ilhhxfqn.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lonidcgu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3efughljj.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jehyatut.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rkgtpwrl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xngbdzro.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qwddplgu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mtmomnxx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3bwkzgngw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfbzdtdl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3koepxnmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtsiuifn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3iqsxmvhb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3mqpcpdan.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3gixwjopm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3htiqomqc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3abttxvic.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3sjcvblfo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uhrfizae.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3oavploav.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ynoyvmhh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wsnaweek.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3iduecrub.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3fdwuytbu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3voxgnonw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xkadnxhe.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jnwnrdfv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zeopvdbz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lvvexlde.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dhxavudo.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3uxhqcyae.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3frswbent.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cmdaaiim.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jgxkdhpg.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wkhimfxu.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kwbacvmu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xlnzcnwn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ixswfmst.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3fvhrmhkz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3ljvutdpp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3phqmrlpd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ogydexvh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3qowkhvyy.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cpkmvvqq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ruvexkky.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3yaopkcqu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3sspcpfnk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vdryicuu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3aatmvvyo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jsjmeshb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3vttordee.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hmeefixi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3qrwfotns.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vcjawrqq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3kmizeent.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ngqcziww.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ccfsfumz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ddglfiui.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wcxprqku.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3fldgpsfy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3knbjwmro.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qonqjaym.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wzvnctut.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hthypoww.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dfkvlevb.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3genuxhby.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rsgieanv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3bxgkrerc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kuvyowth.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3eguzammp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bqndhtdh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3rkgslffh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mwzhqpua.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3guqckpjm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3zbsoovri.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3bcoryegg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ifhxmbtw.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3anstbyym.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ltblqziy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3oxrqjazk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3atmpknri.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3scekkwmq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3odxghswz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zebuvdtg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3xkddmzvd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3tjbcdnhi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3caunbpsr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cmvolipz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hvjrscmh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3jglknbmk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3elawapns.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3zwtllphw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tkcnvzft.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ulgptqed.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xglgtfth.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3xwvdwspd.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fowfshlp.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wljyiedt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qxdnkbpn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bttypnmn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3etxwpepk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3jfptgrlx.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3vgayvstb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3zddtyrxn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3manizjfq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lxpagldf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3otgzxldd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3dvpadyaa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qepamzqu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qlqllrly.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fiysvegj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jjetcohn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zlndyozr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3mxxmfdmj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jtojbvxt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3alflzgvc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3afwhsyoq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3nktfgbzt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mdmueswd.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3doeordvh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dzdbtmyj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3yycetsxk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgcubjbd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fzudvcqs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttjfjzgf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3frzysqew.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3shezfqab.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3rapeubxt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpqkcpxx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3cmqmtjwt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3yakjnyha.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vdpxvlji.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3tbuscjek.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vrfwwphv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lhzbwaah.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3zuiqynje.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3nesfhbed.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vmqiczdd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ijldqqwy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mrwskcst.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lmlbioum.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3sbnsjeiz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vzdwvqmb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3bmgzhngu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3aznqcgmd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3blpdtllz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3uybaboet.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3utnlrukr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yylmcqrn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3hhimislv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mshgejfc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gskxmjcl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3escaywln.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3cgghwwyv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3cyqavwwo.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3evewcywi.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3wzcuqdre.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3lgdsthhj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tevsymqb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ztjknoox.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qexkrghi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3kkfhnxph.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ancjqufc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3iyofxdnk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3niiekboo.html


<!-- 参考信息 -->