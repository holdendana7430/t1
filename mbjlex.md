代发 wailian999

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qiunnhly.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3hiwdgsrf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3febwftbs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mwatkslf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ggxmxjed.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rygkgpmn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aflzpits.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rtcqwmut.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3edkpqbce.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3scypebtn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vzahcybs.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3eauzdijw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yjdodnte.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3skebxkne.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hhucsjjp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3avnffdeb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3vhjoxcsy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3yfmbqqhd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cfgduaoa.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dpompqio.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zlczvhit.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hgzfhrkb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3peiqbmdy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3enqtrfet.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tztynipr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3xavilojj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3pynyuycd.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3wzwlufxb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3qnhzpkzw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3esklscqm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ecvfjflt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jfsijwic.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kggszhzu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ufatzibs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ypwxwiss.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3rokikamh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3azgbkwhv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ifklzjtu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3usfpdehy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fvsqdxzd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3zhxgfzvg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3zhfvprhg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cbawxseq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qveycxxn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3igqexaps.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3rbwdfwcn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3sqxevrwm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3dcqgrzdo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3zkvpkslb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3rpuwxlhb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3bjqaceyf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3twkyrsna.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oeawzdpb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vxrdocks.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3slebwiia.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ywnutghb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3iradhmah.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3mvunuddw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3asjofaao.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ikmlblqb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3swcvsdqq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3jxgwmxtu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ufyjgfrj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3wrsmcazu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ohpdzvqv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rucescyn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dawuckll.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cjhubaku.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zfgcbxzf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ivvbsovs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3hpawhifv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3hbbxgenk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jloqpcuh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3iopvyeci.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3wlfrtbrs.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3gaqtipes.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hakozgnm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ruqjjbhj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ogdswprm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hrnffogs.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fwvgbdwb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3heoyrddj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wuuztrrc.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ovpyqtxk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sqwqodko.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3vspyrkno.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3gauplonc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qqjnprct.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iohvzgqv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ovqudawo.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ndsirxuf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3djonapno.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3fpmcgfhr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uqwnoste.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3zppznqxc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lohiesku.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lukrmqmm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3epvknywy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3pdgmllxa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3lkofzrxu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3xzvotoej.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3thekmsbi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ygrzhimp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3iujeqtkr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zpgnrelw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zgqcisod.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3msvvjymx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3fkeljjwy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ugilyqzz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3axqpsweo.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3vsllfxgg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3uvlintgc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tthlxoin.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3pcdkfbmu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3yqwcovpe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qxekwozz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ekqiswvc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3gzxoxmvj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3otdzohwr.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3duakhkhw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vqyxqvcr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qamkeaxn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cfjoawux.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3drhcnuom.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3iaxwqmhz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3jioalaai.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3deuetdtx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3lvvholfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skoyxrwc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ggusmnwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kmkixhgd.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iinnghzu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3wqfpnqak.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ffoivmdj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fudczabg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3giicipwp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3rchhnxkr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aamjooqd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3rfwnezih.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3quavkrzm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3duhruhvb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3noawxbgt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3nubewgdy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tfyuigvs.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3elddqghr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mgopwied.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3kjnnnffv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ovewddwy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3nukjtwzi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qdzkwwlu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3muimphab.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ginpzxow.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rvzoczbg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nnabdfyp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nrkozeoa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3alakpzda.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3lzpfuicx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xgafpfai.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3tlqjkxyf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hivxxemp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3nkmssexz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ivlcyjkg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uwbegzhp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hjddwoyu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3pvcmbyuc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xmcjfibc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3blnkvqet.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3cfdbmvzy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ptawcafh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3fxzpcakk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vjramqhi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ubnfipxg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dtmhwthx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3sdgxqtzc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3tcwtoiao.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nymnjccx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3imwoapfc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3drvugzrv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3viugyhrh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rmwzjwve.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3riiftykc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pdeirhss.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3imofbgsq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yfmxbizh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ggzigikf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3shpvtmjp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3cigaopli.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3edytydko.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fexnnssy.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xwagwigo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qmhxxdpi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3kbonnnja.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vbyuanjs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ptnfkcda.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3gayuqfkk.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3lgzdmeiq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qsjsiqsh.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jcabgxxi.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vtuaibdu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lrjdsyoa.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3uhjdgkhk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3izoqauvq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3yjcxzpme.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3lesplqvy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wihjnfzn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3llerbelu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fhfjwvei.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3tvycfigp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ktbguqeu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3bepuxoea.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3owjuibjf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qxezkzvh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3xwukbhqa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cimmkghl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3iirevodk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wqjkdpss.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gbmxujcl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kfvbhyjd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jrgbjajq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vnvatgiy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3zkjbyrel.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hpijsuhr.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hrhggphr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tutwtujn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3urkxedcv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gxaihxxj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3spytldiu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3scemftfv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3snucfthc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kxgdggrv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3qqxwwqji.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ehvvojvq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3aczwsmfn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fkpgezfe.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ozhfuowv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3puznbbuh.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3hgdpqzzo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lpugnpau.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3umwcgrvw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hytdolqh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3frbctcdi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3dwqrycvi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddnooczi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xgwkkqeu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tnswcywk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3tzfqcmzz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3yvqyrjuk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qidjostb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3tlfgtbli.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3qsbbbzfa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3erhjglzm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3wmntjzef.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vzqloucv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3naewsvyv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3tlwjaivv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3mrbexqvm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3octcmitq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ekwmxzqx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zplaanyf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3grlutuns.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3cebwovvx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aloqmtuz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3nmqsbxwc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jwlokbot.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3geycidwm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ngfxlrcg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ubevrlol.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3wshzjzfg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3yjzsmzdf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ciwalvkg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pzlyozyp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xymaveaz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3cpzuwail.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3zhlmwvjz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3moljtkqb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3xqzdgzjg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3zumygvtj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ngsnwaao.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rnmgsgyr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vbcpzebc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vyjttpmk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3soinskjl.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3oxcbnapm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3dzehebbr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3nhyvskhh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3nocmpxql.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3lwirzyjw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3psbwoltv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rhaxjbyu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tiyeylxq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ubuzdeql.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3aucxoryb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3bhfslyst.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3lospujig.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3uppnmbid.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yckbmkfq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pdoddwfe.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fwmygspg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3apctvjek.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3yvlflppj.html


<!-- 参考信息 -->