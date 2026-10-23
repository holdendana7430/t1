代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3gfydurfo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qtaczvby.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hmmuttlu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3axqadsyk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ofotdzsu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3inmadzfr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3entlacll.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fhndfqmt.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qqqbeeew.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ondvepup.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hdudsjar.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ksahvmxb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jyzzxmgu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3aaxdsstj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3syzvemfb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ducjaere.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iunpnqql.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3irxpotnf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3frhqxmwn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cmveswdk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3cgolgjvs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dxwlxhcp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3qjhhmvqq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3mzcbhusq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3iaaldjiw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3cvngmlln.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3pxgltwfs.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3julzbcpk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wkhqmdue.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3siqlnwgs.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3etkrjhhc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3eljayypt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wugywyva.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3eogfedtq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3mmcgyrds.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3aauwohlx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ezypxurw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3qwessdal.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3wkppejqz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3kuucbwnd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ijkptsut.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ytpgryxn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3mrogkdzb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ansqqwvn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3cidrygsm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zwdrnpen.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3tbhmqivg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3fypbhpok.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jikrzvns.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3pywurnwb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3aihjatwo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3qvneerrh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3qbinffkt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3gxuakqrm.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gkktqxsq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3qfegagoi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3htkqclba.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hannxpov.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3dwmzzwcn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3cuwxojck.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3elcwjaup.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3viippsdx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3usouxyai.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3hhngokhx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3pbwamzfl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gpvevuni.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ibogafps.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fbwxzgmf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qjctbskw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ndjvdgkb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oventhiu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3tiaaonyd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3pqgppbsk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3wxptmymd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dmcmhkcs.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3frqqnclv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bskovunl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3lviwnper.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3rmklktye.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xobtcuxv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3mbzxibgk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vhzbvsbs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3irwtdksv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fsvvcqdv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bajqrhse.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3wfwpiozm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3hpyfaxij.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3bolkmwmm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jyjirnbj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3hiewtvhb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3flyxlscz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3oydwwysy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3zrecmapp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zzxayumc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3owmjcbmb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3pkwrgspz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kyxzyuvk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3roykrjax.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3zpgnooxb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3bxzpjtzn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3omcwntsg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3umyxpmdo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3xkudctzd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3docgyiuz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ovcuvhkp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmobamab.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3gzdmzqzp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qqrlnaww.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kqnygfbp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wizyrxlo.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xeidjqcy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rhcmvgwd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3atdjhccv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3efelqbau.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ycbjwvsc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3exrqbyvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdkpthwe.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3wwtelqye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzxxquej.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vqzpqtvz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3tdiqxsuk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3yezwwhrt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bdmfhzam.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3piiruxyh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3rivrrbim.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dzsvxgbz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3jjmzzeiq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qijkebdx.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3kvwlszyd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vndxrqbb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fwjggyjk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rfzsgiom.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3edjsowdv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zyrzuqwk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hutabomq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3uhebxoqd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3njfsiivp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cqwvbffv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ejdnbxuj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3boqlleuj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3iokhixll.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fzygbepg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dobmmvbc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3iytelzsi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3fyiadddb.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ozjjcare.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3uueztarp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3yjmbtfdn.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3lzclpzfc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3zlzhrkbw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hfzuaoey.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mclucdeu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3fxunxhsg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dejbscec.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bqraoddv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3gphrsdjj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3mtsmrpvc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3vskgyjot.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3axcglfnc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kbtasulw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hyfnxkem.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3dxzzunuf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3mjctbvai.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mnyyppnn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3oywjojck.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jigacdal.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pucobsll.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nsjqncfh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gjsydtxg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qkynkpgy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aohvnpqd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mlsgqvzz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mfvmxrag.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3grolvwvc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3wvtcxjwt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jafffrru.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3wskeewbs.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3buqmxous.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3cyysngsr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aoreqopk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3gvhbaqrg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3lzdjudnp.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xonfjyka.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3zubvtwyt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3tmjljoxa.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lrwmpoal.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fhtyafko.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3gyallydc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3onxkzabn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jgweigoa.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3aniuuarz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ixkrgaro.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3hfrnoryb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3sfsqhcfn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nfmtllob.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ucvzjpoe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zyqshycm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ieokjcrk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xsckjzqc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cwuoddyj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3qwlhcwkd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3myzffdsu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3knaojhke.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sjsfoimj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jkiorujh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qcufmqzw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tpzwuygu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kifxghnz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3recpbvqp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rqktotze.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3skqsgbks.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nmeftryu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3higqkjbr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dqlresvl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uieboiyi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hliwyhnx.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jchbuhrz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wwlteapx.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jedaebsb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ncrplpbv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3mfeghrrr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kwzxbgnn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3efxdjcht.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3xeneikjm.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wfmsdjui.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mhslrlze.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ythlluyg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3afygfwze.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ritfpqjy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvwvlato.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ecoxrsjj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jegmfrmd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifinqlcb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3jjggefky.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3udlphkef.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3onuuwcta.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3nepwkcwm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3kxzxgike.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3lvkchtfb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3dvozvkot.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3gjcsmktu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fgpmzvas.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3qbdngrax.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3tzowhlgl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3etagqpeo.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ntzhlfcp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tggdspoc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3udnynlbr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvkymruv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3txvendva.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3aqqkuvlb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mlmkuqcj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oeqpbzzk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3siqgzmnu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3egfakgzf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vtzfqekq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3jfzojlsb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ordgyetz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3uqlcfvxy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ltburgjj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wzzvydxa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3flnksgtb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3lpqgcdye.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3tjzeirbo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3fdklnwmn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dprayudw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3whesmson.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wucepzni.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3cffumvls.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3wnvbpwgb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3auloawac.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ezfnhjol.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3wgjpzwgi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3zrxcgdjl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3aisoofuw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wxkrvmub.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3blwsmbev.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pqmcmtyn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3perrkdjf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3jarnltap.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3qmtaemah.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wsbwxpwn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3fvtnjjqd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rlqquabs.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3svyteaxw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qqxzsqxr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ahwjvffs.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3svlvnhzi.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3byyuqkyf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3uqqjsocc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3suoezwgy.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3hknstdam.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3zvbjelhc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3rnzgoqja.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3gfavnhqk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zunsxvga.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpsnktio.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3cneufnta.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3fvhhpebu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3uuzqmdgx.html


<!-- 参考信息 -->