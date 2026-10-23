代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xqexjabf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mmsdxmhe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3bvujitzv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3xysrwltt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ehjtokpy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3cqatermx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pultgnxj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3rphotjfr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3wwfzuqsq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yhdtbhgn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ylracivr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3eihnitaw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3imnoqatj.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3wyzyaokj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3mkpkuyrb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3shdfzpap.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3kzalzttf.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ejscioxn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3huupzslf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3sbdugthm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zmvjecqk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3xbjcwuxi.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3gyxtmcso.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xcbhmewd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3bxxwxmaz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3etohdkwb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3omtaznus.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3jiytrigp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3idfwgwcz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3jibwngix.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3oivyvriz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3heevickx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ncwseslq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3qwungfam.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gfwanaez.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kcichsdx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hinivfls.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3acywesfa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3pmjjsxcy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3biebfzym.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3brwxstqd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3piejrnaw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3rcfnknbb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3kwsdtlyr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3diatesbx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3idxklkez.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mrsiqzec.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tchlezje.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3omtuzyzu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gdiscosv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eyrkztof.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3adlctfrt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3xbiskxsx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3cxtzrhxb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3fvzhxiym.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3jrwxuvmb.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3khbcfnyz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3pkvnvmbm.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3dkdrxknn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kkphnmtn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3xijkdzqq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ygyxbupc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xfijvvnp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3djgvijlz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kiwcekym.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ajjmqjwn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3feoybbgp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3pnjqzoeb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zitbhrjq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3vbtymqte.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gtfwofjl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3iutsjgqw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sdmrvllw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nyyhyypa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3kwfvzhsa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3dmnekvoy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fgzjdkqt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3dwaizzia.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3pejqqptp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3bvntkouu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3jmkotxkk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zllohvim.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3avheztmi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vowqeprg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3bgqnlnpo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bhptdtgb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pqurykkf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uuxbnnux.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pcdrjzul.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kdfyxuem.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ffzjvajq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xnquehjd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hnctqteo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3nnnxhwyb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rajlpnwn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qtnwwicz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjjsjfhq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3dnkzkwsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvazjipo.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3spuwteil.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3xlqqnvqf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ldxrwjzu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ldiuhaie.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3uiqkmlrl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3fwsvvyxe.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3wsaespcl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3gpxlzqot.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ofdwawjw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tvcnketj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xbcjtoac.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3fcdcmaix.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mwuutoct.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vitawbdf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ekrjzblr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nnsggkjv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3flgipadg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gwnlsjls.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hjcncbrr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3xkqsogmb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3izrhiblw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kskgkxfc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ehdveyxx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rmddsgyf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rpdijkxn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3yuzikara.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rvnxgjla.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3lwabhjlu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qtmnjyow.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3rgdnerke.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ktmzvqki.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zjlswbnd.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ahkmzcju.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3awcidmhs.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3juextqyy.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dkubzval.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3yxqcxzrq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3blkqwyvw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ydfyoenp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cydilfle.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3dsvrdvdt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vhegwmqa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xuwaypjr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3mipwpxin.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3iklijldn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3tnbnjwqd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lnjrraku.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3wmrchtqk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aamuywja.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qwpembcd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gfhbptqi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dvlvvgvz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eexblkxp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rdkxjtsh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3rujofybf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3sjpqccnu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zheswczw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ttpigjhg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3aklmltpa.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3xtocuuvp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3usdwvore.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3nrrwgnxe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3fzdcqtsy.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3lrneqpxa.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3rdvdlbam.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3xzktkdqx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rzietjrp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gfblfnoq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3buaupssl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3hsxujayk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lddgadjq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lmjalvbz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zqbtqqrl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gpvtxhar.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dyfcucdo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ftfqtwkg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rvuypjio.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ghexyexy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3equfwiym.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ghcgdtcv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vtjmruod.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3frdyqvty.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ldgzkzhq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3icbqfhpu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vwwvfrxe.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xmosubwk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dpkypehv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bvlljkes.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ueknryhn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3cyjcaxqq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ofhvdomr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3sohstjxd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ffzhyjzf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vqvsqcvx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ibhdqgob.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kqzadgeg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3yserjwjn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xrzzzshy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ahjxaxtu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3welpnwnr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jmjcbvkk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3wdgznazw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3grymtvwg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gsyfqwhc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3izvojccn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3fqtaswmy.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jitzlxzf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3kjfeooix.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qqxyrdbu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3eramogyu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3lorbxxcc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3llgszhyk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwzzjecu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yrjiuurh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3srnaoayl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3trkpqpcc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xmgoucrr.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ilnhdwfd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3vasrxiuu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3arhgynys.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3xiurvcjr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hdbxloup.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rzxsmfvt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3vnmulskf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3wowwbbvl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qortrzzt.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3mmnxatag.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3betrmoyx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mpusbpyg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kjxnarji.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fzeuidyv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3yylgwvtx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3thawygje.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3btxsksvi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3aybsxdou.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zwvvjglj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3queuaisw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ytkwkett.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3nphdinqf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3blpkwtsi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3djrprgfx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ltetjxij.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kmrtopiz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3blnlzsel.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3aeaijxkk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3xmscimny.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3pllyszgd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hzivlmlu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3votmarjd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3fkcmjgpt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ujshfdew.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3fllnyhgd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3pwwadswr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3lvydgpbq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3glazdeix.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3rhjfkzsq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hluunjyr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3abfzoioz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dvylozza.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3moglglry.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ylhonjlp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fliqujet.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kubylckz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3hyrcfagb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vmufxtmn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3avoufuji.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3dtufvvua.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kwviocqo.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uiltyqix.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3dkbjkvej.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3tgrfzirx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3nilkgypj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3diwkjkrf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3dovgezib.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3gyyrzbqn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3dsifrcit.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hczhzual.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3fmsshhoj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3maawmram.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbriylqd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3rovopgpw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3vteprugh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3orqpiptr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zoadsdra.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ntdvesvj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nekdagbh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3afcgnmxg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jlnwrwsn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kobtjscg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3blorelof.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ltmnkbrs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cokejuqn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kcbcnpxh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xrawnplx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3uihrlmge.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3nzjumjgz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wtctjyal.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ncdvnayl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3virtbfuo.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ldldqjtv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3chxebwgx.html


<!-- 参考信息 -->