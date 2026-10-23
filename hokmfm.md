代发 wailian999

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3lacsyszw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3wbiihwdb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vdegrfgj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zbmhrhis.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3abjdklrc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gdwdhows.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3koqxjdtm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ysppkqjq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3fbxybagd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3qnbfvgsn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3hmprlgzr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oayauftn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rnhdzkge.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yzmtwcte.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zrbbvwjj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zkkgboxc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3eknlrjec.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3abywimwf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dvdbkjas.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ckogvpfh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3izpimahu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3udzamskz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tjuqyrna.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3eqcdstdc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cdundfqw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fvmmazbk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ykiucscx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3raroknkd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pnbowtbw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tghbvopy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hgnwaunc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xxacoxjf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uousdupw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3cdepcsod.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3apnjwqcb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3jmecdvcn.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jipwiddc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ptewxmiv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jbolkybc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kjzxjzeq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qzpvqkug.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aljumgmu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3hpcbwbqh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3xwosyhel.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3aukupygt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3jkcpytkk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ehyqnalq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3prdioqyo.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3gqttjlku.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ifzxltir.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3putibuna.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3jrrvolop.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sfmfznma.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3nobfrmir.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3migmtajk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3hlllrbrd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3klbcuwhl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ojgptjmb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3amznsynj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3qhljfnhz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zzwqpdwb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lnrefgar.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3vgypkphz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sjkxlaav.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3nvbmaboj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hzoyjixa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ycgiuvhz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3pqpnysqx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zwoaktxh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3aemsyxqa.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3dbvttihz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3neaetfph.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3efmdsomm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mirlubbf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pvmokjgs.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3voyomjde.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pyloyimf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3irvzqwol.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3jhnytboi.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3rewboiqp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jinzcbfd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3amzgqbfh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3jynjtmii.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3igxxrpul.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3fanjetnl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3woyfofyx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3awhjswpv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3treejrbj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fdtyobry.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zhiutbxn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3neekvmnf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ajpfgqzf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3wyhgoros.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3zyvmaseo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3lfrvyodo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3afcaqzdw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3urbyqkbq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3pszgmsod.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3pwwchdcv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3xgqlyeab.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jzxtbikl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3yfknrabl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3fatmuszf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zsdqijxj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3cipiddim.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3mcsbuhhj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jbgdpjoc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3uysywpdu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3oekvhuqs.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3wmzxlmdr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3vhvutafx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wuxvehyf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pnjxyleg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hwrgnesu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bvzuxpqb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3vqfpvgwx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ecipfvgj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3hjuypsbx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3tbkrruth.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ugcctxwo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3flbnwiny.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ihrmyjrr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3mzlueutf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ahxfbckk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3dpnfynem.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3fgavaktu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3icnnbsbh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3huljxlpn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3hdvuyctf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3edlbgthy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lqxgyhji.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jvbahahl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xcwwayka.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sbjqkoyr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3peameahx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tpyhlref.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3harhimlg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3tvivkqxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hsjaajql.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3inrhgfhr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3bdmqfzdy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3naeczyao.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fqqsxtsk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3hkyiqpsh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ckypuccd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3rrrupuzi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3cpslggpv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lbggjfqm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vkdkbknl.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3opycloty.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3odrqxqyz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3isehblbv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wgakujma.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3njsibsxz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hjeqgkay.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wnhuoudb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qlqrpniu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tzodqwtg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3pncqxikq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dczoislm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hmacommh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gynxucjc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ikilwuou.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rdscmhvc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3fxcdhukm.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3bxzlsvpe.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3zpayvphz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qzisevkk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3jxidduln.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3inicozqu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3znqqggzs.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3auehfucs.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3rlljotvl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tvvazeul.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lcshllke.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3uoizlkml.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3byimginy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3hohbhyzi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lyxgnhcc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3giptjqby.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uhogfxlt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xeecbtiz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3cldbtymw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kgdvxcaj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3fwpslcch.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fmlszxeh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qiffmjch.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xydlgctv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dwgokbgc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kbatnqjk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yoxppifc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dttxilyi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mldgmmqi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3qmrzglan.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3gzttjemr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wusvgfyo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3mngqucum.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3yuhfggyd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3tnhjywqt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ehorugcf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3lmxtcriy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3bxilevtg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3dbyloecb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3yqdzfmhn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3jomoomtd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xlmdavsl.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vyafrkxn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nxarqtxb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3qxvlzqct.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yxeeznzn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3khaponiu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3rcdwwzel.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cwhrvrts.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vrmdcogr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jezcwmia.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aqrgqkfe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pplriiaa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3hkgwsobq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rfjraazw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mjogazdk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3lpjrsfvh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lscogybn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3clwjasrr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ezrzpyua.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tcxlrfne.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kgpoilrl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ujcrahuq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kxnrawwq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3wooawpsp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wjgusgvp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3yeaprzqk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3seoztcch.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tcqlrpxa.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gwfxfbdd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gwajxijy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3yuvryuwz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tkyxnzzz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rwwiepsp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3eplephpo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pmwjumet.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3fmpzqudu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hrfkcjdy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pkgmmzhe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3vifucwnx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3iicnkynp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vmyflees.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3nasptrwn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rfcayood.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ehfzqmzz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3discdktd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zacqpioa.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jfgzlwyz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhcpkmbm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3rrgqfjnq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3mohcckva.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gyowrhvt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3gaxufmhv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3whwxmtih.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ktretqde.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3gzbzdaii.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3xjmgztvp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mhxzaujb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3shkozdup.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3viukhkrx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fckublgn.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3eciysvsm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gwqccogk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3utvpmyvy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ejzmkbrp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3lmdleccq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3anhwritl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ydhrorce.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cononbtr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3qdmamdli.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mbsdagcn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qrbkspyy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3hsdqtrlg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3sncpmoqs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zysiheoq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3omiencju.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ywfsjuhy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3einghxuk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3sgbovrfd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3fkodvajs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3fmksbxma.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3towdoikb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3chzmlbqw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3owxipbjc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uewcvyoo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3heqrdgwy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nfidnzzg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3juryqejk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3xuvsvumi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3hjfrkxql.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3dwdlxmmw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uqcvrodt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fjdwoeih.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qevsuzud.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3smenkqjj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3yrmoplvz.html


<!-- 参考信息 -->