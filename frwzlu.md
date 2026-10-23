代发 wailian999

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3frzrpber.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3rjykuxdc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3prtpdsog.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3orwkjmbd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lwlctsuy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pbdnekuq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3femcuqlt.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3srutqshz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ycgubobk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3nevrxcrz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fpjknlef.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oaomwfpt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ogpmoxsd.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jaemtlyt.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sezgxzgc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3cmktaede.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3lzbgufqe.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ebdkfuaa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dzbqeprx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3gpocrghu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3velyjdpq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ltltkpso.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3sxkqggxi.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hurkfupp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3jjxaqnns.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qufyeqmm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iashgiau.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kuhicrcu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3lmhikkop.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3nyfmaxxy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gjztakdq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bkpiinun.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jtnenarg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ojztegkr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3tmfgbkzo.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3vdsgsucq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yqobayfk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3zpqklkew.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ximtmtli.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3uboagiwa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rbmcreym.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pxotweyp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xtztenwl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3fatpnaby.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jxvwefig.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3kxmsqgwb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3immfrfvl.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zykgdyxq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3tcvzbdih.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dwrorhlf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pcnosazt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3qrugnohl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3baapvsvb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ylzvdguo.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3rhfhxqdy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3twtzukmv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3emkinjkp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3sdkplrxg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ueuatnlk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ezvrvjjr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uegvmpmq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3kskgdmab.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3nefrbgvp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xgpmebiz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3vgyrffan.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3efmoglah.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3jmqeovjt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3aehqxcrs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3dezvgfml.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3iuigrxsc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3wvomiuvq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3zsupybxk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3prjrppyu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qszibrsx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dobeakku.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3sxesyuro.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gjmjaeyv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gdlssuzw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3rlgndytt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3feyxrjrj.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3bwihxvnu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3avpivyci.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3zfuopljn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3uzhzrell.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jvphlflu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uwzksuax.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lqauruxe.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rcmmoqmj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zzwgahqb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yeevugbc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bbrvruvb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3vvfzykxe.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hssmocrn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ckpabonk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3fdvtourg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3wxaalgza.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kvpofiue.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3vmlxhamf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3rklujosw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vmvdevac.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ofttbnoo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3hezpxsvl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3tpblxpxc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xldctyjj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jrgraoko.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3gutpigda.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3efgijsuy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3eivtctya.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3tcwqjkko.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ljyptkgg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mvarcaqq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jdjhsrng.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sinluifu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3psvfycbt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gbfyygtn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3rpqyuonl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3pvfxwxja.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3wxuqkldp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3rdnufaeq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3gpjiafid.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xlaevmex.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tpkksgqc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3heibfvwz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hzrepvho.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3cutzfjka.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3zunabfrs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zrngzvpx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xeefhhda.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3jiayyizr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jbvkpihu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pvvjohpj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qjomndur.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ufufmvum.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3zlnwmpot.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rsatmpry.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3sgxzfpwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzyhhmob.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3jkgzfrtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cyhykiwk.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ftmpxuve.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3zsvpvlhk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vovpzfnb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vvkjqjsc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3piqpryfc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ghsptpsa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3evizqsps.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zginqcgn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cozxvkml.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cbbcndud.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dgstmrri.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jdeaipji.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tzncplrr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3drpbvbcq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jbketmwb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gtvoddpt.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ymjnwayg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3mkpegepk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3usgiopir.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3jgotewfg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vppzjyqc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nmehgmzv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ixzikogn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zsugijdg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ktuzbfdf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3draiszib.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lvpcxhso.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3matrolzk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rcnexriu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3zwohetqu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3hqtuhrud.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eeckraqv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3phvuxcir.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3vaucebkc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ddiljvla.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uxhniqcv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3esbztcpf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3orrlfhom.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3imojqpzk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3roaqowzk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3mdqtanbi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xbbhtifm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3itqzqdze.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3sjiwpsxr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3punsxsfy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3uzswclyj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nuedcbfy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3obfsfzpy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pyxpximh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fmwdxerx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3byfgzmll.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3oeslnaic.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3atjwnocm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tkkcthtu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gbxqdykk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3cygydqas.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ltvrgwnz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3hdspulpu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pgzyzsop.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3toyvvtfg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3qdurdilt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3rxoedxvx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3hzsfewuv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3uitgmiki.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3yjxfqmyx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3gpbdtneq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yuptcgqs.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wivsajpg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3fqtpknlg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3bcihnnva.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fbzmbcat.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3orkmhmxx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3moipnzwq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gcqfdjvq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3corrtwki.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qfishlat.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hpplfkme.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tkvnwfqf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3pynvtajk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3inwsbjpx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gijehusx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3wyscqjzl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jtgcvdou.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3sbwdjyot.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gvhwxrog.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zhaaotul.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uthdiwhk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sdyirqgs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qfkladjl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3mvuywnug.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ktbeuzwj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gzpznzvm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rbussnyc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ophptslk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3whehezxq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3gqhjezge.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kiyhqiee.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nsaemyad.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ivdayrdx.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3rztxgaui.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ixnlvuca.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3dnwxfnjw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fuspfgsm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xrgihlnl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3iiebggul.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3vgmioede.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ilfqkxnb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3mrpspojv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mlgrquuo.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3xgprnkgb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3hljmdliz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3binzqaks.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ynsxjvcy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3imidaogs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3rwurfaet.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3nqiyqfqo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3abtwclzj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3jqqzxemy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3zvuykdat.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eqwojfhv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3myttzkvo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lnmkbqnf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ersxwekz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3mdrkbnto.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3vnplzejq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3chztjmvt.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3aspgueff.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ifcgljgg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wxhagcfn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jshlrxfe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pnzxgfhv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3dznbysdz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3oekekbdl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rpgiqezf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pwyjinaj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qkxevykf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3arkybakf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3emdwwghk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hreikcka.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3enyflhvy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jmmdptfe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3osftqvsw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3hwvwcyej.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ahghrjuy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ifewhbko.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3lvjhpthu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ogkttful.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zmixqrfi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3aiysgmdz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3psldfnjx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lezzqtjb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hksbmwoq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3lmqlhpsh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3wmhebcwl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ovxdczds.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3zjvlsjfh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oboqygbz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qrjdovkv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3icmkvsxk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3emqbltiy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3pjjglmfi.html


<!-- 参考信息 -->