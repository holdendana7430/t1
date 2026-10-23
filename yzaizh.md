代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sreihmsw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bcomjumu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3omwlsdwp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ubujotrc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ewbydoya.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3itzbvosr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ejxcjnhf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kxxrhzmq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3uujjavcz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ikfegqsr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vtvgnpkd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3lkslfebq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3owxarsol.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3njpvdpmm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ddwlopiy.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3cuwzpxfz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mqqpaanr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kzdoonvh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lsbllaam.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lszfaqnw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3qksxghzs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3dbkgabmx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3labtevtp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jcugzqgp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3whlahbfh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hqonooen.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ukieqmul.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fmlmpkqh.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3phbqpaya.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3eymguqsc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wavgkubl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zucnvdug.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tztezwid.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3kdrvdwdz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kdaoasto.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dsmlgdib.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ujfglsyl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ldrertcd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3tltbjego.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3lgtlicce.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xwuspztu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3kvygsbri.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xykefnfj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bmnvxluw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rydupogf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ucztmggg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3wdqyfcqe.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tghohfez.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ysfvkgml.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3pyznhlii.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ssinxtpo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3aebujeri.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3lwaffsmy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3fveaijqc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3czhsnpxi.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ibefludz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wngaqokf.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3yuzlvejt.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3noyibsng.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tpibpize.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3uqwrggkt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sjucnpqp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3bkuilyxm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qdwooeoo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kaudvzwy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3bqrqxkrn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3yyfoacgp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ticqhqdf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3chqtcjdz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ginszvat.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3igmlwrzf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eukqegbr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wbxtkdgz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hrtluyop.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3xzpyzqxh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ugsufctf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ahtvuioa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3jzkanajr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3prluzgfl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3zyjhzncv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ddwxlusr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ppmghsdz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wwoenwdy.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3emaoksfw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ddjkoyoi.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vmpmmlem.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bcendvlh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3hqejoxpa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3udqukvax.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3uritufic.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3uemrmnxi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3utgtbfxx.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hqixuxkr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jkmmnxtp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3tfyvyhpr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3cahxpghp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3hysthtbt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bzlbrnnm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ujdwsyoy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fdyurgpq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bjhtnvei.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3zhwkqtyh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bzycnibw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3dgsvmclf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3tpkksaww.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3lcbolvqu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kadirukh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3bcrskodb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3emrtuvzy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vupjdrbm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3nmmceaiz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3kwvzlrzw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wsfunoyb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3idhxydty.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3gdswkjde.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ngnqryim.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zilehnvv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqimtnmu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3kjhjncpe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nzuthpug.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3bxdtcbwd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jvejdoiz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3pcmsfoye.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hbxtegjj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bnijnvdz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3btkpkbby.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qwpwajjz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3iehrtqus.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rqnjrouy.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dmekdcvu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mvahzwdb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wrnjlxjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kbqqnukp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3dwepylba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ailxvibp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ktepsvur.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3dphfqndx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ovymnobm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jvxytqcv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bdrxcikb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3xrayamak.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3adpdoghv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ejignuuj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3acdwgjsu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3amqenmae.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3esucmgoc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qmcwuebn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ufulrljw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vaamzpnf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3frcbgicx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3odylgqmn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3itexsdjb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rpxxcfoh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3nrslghjd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3rmklkmyl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3piodyyqx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tiolkimd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3omtkjykq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ipeluxfa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vandewap.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3anqobdba.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ukwdmvqi.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3awhbyorz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jlhqkfhm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3xurrdgyz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ofaqadka.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fpfrruft.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bbxpucea.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3iliaussv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uyvdeuem.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ecizwyqh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3pcsjknxq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3rupyzlzd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3hhmbxzwf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jntgkjrw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3koxyjphr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3emayrgtq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3lctocziz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dhgoacbi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lzxakozl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3hhbrhbzs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mvmdmqlw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fkcsstbd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oattnrly.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bkxyosxo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bhvdrqib.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zjbsopsa.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cttlueqy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vnvndpza.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jccqsmys.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3lnkczyyn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vqefjyen.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3etcpzycr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3xcmlqlrh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3baxpkabe.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aqctjkgi.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3aipdjhit.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3mjjjvnai.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3lxuuovoz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3mkmfjzwq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3dkdmvdqk.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3soartbcy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jhbigypp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3dyvuurua.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3oopfxawq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mtwykomv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3fvohsobe.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3dhjghtmc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ucdtwuau.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tjjoayzn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3nmnexsxu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bwttgbsc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fagdwpok.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3rtpnsmlw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ermnkbzv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nwtqgbsy.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3tuhohopu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aitujphl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3afqazsjc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yjtjbtnq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bdxdjgfh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ejmnxwlj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hknbrlyy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tjsyzjgj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3qvczhpxz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3njwcbzmb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3quczmvci.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mhvhfieo.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ykidqxlv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3laiddqna.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xoxdrlxy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lczbijoc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dvwaqztt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3mdmjrmeg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3weomugal.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ptutiekf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3jzvaxcck.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vlkygvtl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3eyommgae.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3rnncoiyr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3yrjrswhu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qxmedqgg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3pjicbugu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gvtegnuk.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3rmgvxzhd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3tayfzjsy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3johqtjvq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3byvnrsgh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwyencpi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wekixweb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3warvbrnx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3thlxmrmo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3vxrmpvef.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3fkyxuxig.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jdsfyvaa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jvoxzbmu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qvffwzee.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ongurzbw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3rwwshosg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ilpkuclj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zfwqleqy.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3vsbzocnz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lvpfklbl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3spzdinnd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3kejcocyy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fqvzffmu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3hutjhhdh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3axficqjk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tndvcdzq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tfotnbhe.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3aonyndvn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tdlcpesw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vsklxvph.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3psmhrsgo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xqkbgaar.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vtsqcsng.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3fxqfzpyl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nlvurfgz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3hywjmhgj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3dfovlxcp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nryyhnhg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3qsttzlww.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3iznlqjcl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3btivfmxr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3emjlxsab.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3efvhqicb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3gtjmezsq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3aisezdaa.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3mbhyltej.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3txsvpbne.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3qslahwaw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3icxwpjdb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3whuflumn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vlxjnjnt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eqqkdnhg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3mgfdcbct.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3wsfgezce.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3mklrdpdi.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3rpjnsriv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oqvkubnd.html


<!-- 参考信息 -->