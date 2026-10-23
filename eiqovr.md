代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aauhbdwh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uwvlaacg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xmmxafeb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3mvonccvc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3kebmvalf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3hoajhrkw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sglpohfv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xgbkyput.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3czinopit.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ubzkmqig.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ndnjptvj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cmddnpqc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3aadhdejy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jzwgaozz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rlirnfhm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tuxvneim.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3tbgtaxzh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ojugqwzt.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3jqdzwvwf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lijzxvyz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jwevhyio.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3lafuktqz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3djqryfrp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3xvjfjpub.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lnrphfke.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ujrczldk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3emcacdne.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fkkacrjf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rdziqyvc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xktijrgj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3nsfgtcod.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3oprtbmdi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3gpyeltnv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3xyznvjku.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wzhzqoun.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3manmtgyf.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3raskpfuf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3hykxfbxj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3krcuktjv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3edvpijos.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3axnflebn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kkdtscgi.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3vrdodiip.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qflwmtyv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3pjgmxxxb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3zyajllqm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ggwrrjcb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3hemiwxzm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3guwukrqn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hponbxai.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qoidkqmy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hdtlddik.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3tuegyhvp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3prercpld.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3zhdscutt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3gfoagifg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ahthqwhg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3etqjlehb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3vrnxjcne.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3spqlhypv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3bjxckfnp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3sfhweaas.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3uszirxtv.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3jajrwlpe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3snpptkao.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3kjhdgimx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3neqztkxk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3hkartira.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3nblpbcit.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3pmrfptpd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3yaxharzf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3psghlrsn.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3qumzbamw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tuzaydfs.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bqyjxlhf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3puzjnqmh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3syxrnynf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tvesphbb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aruszjmv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3fgxrbqto.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cglldjwy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3msjtcaln.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xaxbtnou.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3xowkdpuo.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sbicncxg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3jjezpkin.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3enupnvih.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zqcqnjaz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3mjdhukvw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zthvlueu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ydpzmoci.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ffjqvbfr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zpczwiss.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3wqzqwpra.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3cyniqtal.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3kwlwpjtm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3jxcgmjof.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ulbgrtwl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3tynpkmdx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3jywgedgq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3utedrbtr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uixtidfn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wyuvfeyn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3kdqgwibc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vduwamlb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3qbdmdxap.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3jlyxdwnq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3lnvkltsp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xoijtiza.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ivdyymfh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xjnlkfbr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xsnrjjht.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3yglgpmvt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3bdwuiusi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xqprqfoq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3yxjlmfys.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3djspkloo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3skqeawgy.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qbswxblx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hfotjvjb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wqtocyty.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3imkskqgs.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hdndtiou.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3uyxitoqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jaixrmvd.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3lorwiwiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbwnpogx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zhylrqgp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ncdebhic.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ucjovome.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3knbaucmm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cbbvzldk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3uzoiloyx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3mqyavqbb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3yjsfifnt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wxvexqyg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ntdotsgp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vfnjfvra.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3worubtnq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ipmefceg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3azcdtdjo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ruhdygni.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3agidbjyj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mnotpemb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3idybulpe.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ugfsrczv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3lqqsantk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hmgkaxjw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3aobosyll.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3scluvadn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jvvjqcoy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dhsachtx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3yfzflvff.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wfzzzwwq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3xjpvjmah.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xclmtcsf.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3nidwocfa.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3pkoqfnzh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ubkdiysq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wjffngyi.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3iqafdugm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3oanfvfgs.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yzpvyccc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3jbpyvyze.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3zdpqiese.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3iyeuwdkt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3elejycrc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3brnvqxdm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hhsutyaw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3enmuyjdx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ctmduigq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tsoqhbly.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3tjoiyiug.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3mjfaebef.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3jnjkkhry.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bzkayxma.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cchqbycy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gkhbeadt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3esruunaq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jaijbnso.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dwwuyvpd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lexcxsba.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3qtzcnknq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qngnxnqx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pseflado.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ahmuddng.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3pweowhls.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hcxycwqo.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3zeyjpwyk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3wcpvgwon.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3jhgwnmml.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3lvcwdscd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3qcjwiioc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yxyvqqju.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hoyvyvgq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3puzwrgre.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3vtsrmhce.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kogjndvt.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yiqbpfiy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3aedpamsr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fogecull.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ktfekjpx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mimdpvww.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mgtqikfo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3syaehlss.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3trnlhuev.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hcjjdhho.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ifjeyywz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3colflgpp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zyukjadu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3uvfnjarc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sohrtxty.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ennrecqq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3euryvxgv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3spqincla.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qexuvyjy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3gpecnmzm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sqnxqsjt.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3agjyeqsv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mfemfxol.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rshjlots.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gkshsttk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ihfnlngf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3sxpupmtq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ajjmiwkj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3iskfzvxd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ilmfjayk.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lglthhrf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jhrneazt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fmcyqxop.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lileifcp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3vdgzpyas.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3vfxcyahd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lcdtglfg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3wzphusjj.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hgwdpkmi.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3itvjthuf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvpmttkk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddkwhxla.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xxfjvsfj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdgzlyab.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3cuswjexw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3nowhiqlp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwlatvpi.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3zheduilb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3gathlnje.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vzxiuhsi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3upppslwj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wyzyyyjx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3konfbhth.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ybefcetz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3gcmjnseu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3leyfvkjz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3jougqzdt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3tnuzjnft.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kbvjijya.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ikdioava.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3lrvieuis.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3wyfbxool.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3glysmhgc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3jndrwbzb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cnbnseof.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wxrriykk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ljnodusf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3fupmxnxv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3uzyxjkyn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dmtncchz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hvstdrcu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3htyaofdz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3rqqbuxen.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3zlqvdknz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3rcibjtfn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3epjlpvuh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ezbpyxml.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wfetwjvv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tkwqrhfy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3nshqnkju.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3opyegfaa.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qqdcbnss.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3cxpnvwky.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3lawwqyxx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ltzsisee.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ezpjqqld.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pkftsasi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3icbgpfxo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3otgfqvex.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3djmxtghe.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3gtvdzoeg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3kcxdogjf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nzjkkesc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ymqozmne.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bgzckrbt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ibwxtsfz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vgkktrki.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ijypknrt.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3wcxwzqox.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3mjrxanws.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3bauuiwja.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3itlmjjew.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3emtqsorn.html


<!-- 参考信息 -->