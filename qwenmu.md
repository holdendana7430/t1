代发 wailian999

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hemwifjq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3tkrvqipa.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3rqqlgahm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tbxfmuuo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kafpizyv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3whdgwnju.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hlmurooa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3uvvbipvp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3jtcejvuw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3caxmnlly.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vetcpnxm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3aqgiuzpw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mbczigqk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lwatwely.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pymfnibu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qtqltizn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xwakwcig.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ouumiugs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3akplarwl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ythsbpcy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3fkwfwdkk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mnitxtyz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3rvgjosnx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ywzhftml.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3crgflrnc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ujuczrci.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3fnkagmtz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3wotngofk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3yipgyizy.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ulebvmgf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zvthggbf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rgrigxzp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xhrlukve.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3atpgbjtu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3mjjzqpkt.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3gllpoibb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ywzkfxuw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3etjrawyt.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3qddcpauz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ppurmhpz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ctmsszqs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ygzryofq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ipuxokay.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ixesioqu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3opfgunyp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3sgixhwez.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3trpbcqnu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3yfabiysi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3vkpnwvkx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3kuzshghp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3mtohxpvl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3zaomojnv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3fnbypfdp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3yuwythrs.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ollgvjvc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vynpvogw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3oxpcbbdl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3btjxtznc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3sqtovphq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3vnupotkg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xguladwo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3xabuvysd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3rbxkzkps.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ttnroxod.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3lmmwmxcp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3nbegdxxa.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3qhqxqftn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3qxwwxbdf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3umxrwcyw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3bvbflthx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3kvtyhpbh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3kjmehuul.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3kiqkodtl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3khktumnv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3pndfdiat.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kpciopmv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wsybtnql.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tkhobxmf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3apmalwcy.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ifzhxaaz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3opfufexa.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fxfinxyx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fjyqzkey.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3nsryagkg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dtgtsiij.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3oizchslf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3frpkqghl.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3gurqbqyn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dydggola.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ytfktnic.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3hsbvrxvf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3juyeemzk.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3bwrcmqus.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3uvpckmcw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3xnjogkfc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3prjrwynk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yzekfrht.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3mvwwxljl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3bqgepbpn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3zgetlecp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3asvseqle.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3tuixojsj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3wjicvczf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mwieodsp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3krthigii.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zifaurwa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3soepuzgm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3niygeqzs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3daypuyer.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3iegbtkbw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ctsehtbf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3rtwtlwcz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3sxrolhkt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iamnvznq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3pvvsmvji.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gjfrdylc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3jpbephkd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fpgxifvf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vyjsvhmj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3frhskgzo.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yrrxdopu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mhdzhveq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3twuwnebn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vjoepwia.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rklefezn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vccxqtqq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vpthdusm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ycpczdcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqvxmhmj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3yhkgrvui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvarygox.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mojyxpwm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3sbbofkjd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3epfgwrzq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zxgiobpp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3mnlmghmw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ctcbpwij.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3sekunafi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ngkbarhw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3thlzcqsw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tnyreofp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xnqrrbkk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3isyibgxb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jkuthznu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mdtmijgo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ppyprebq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3josrotvy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3csxzlzgf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3zyrurizk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3uvqyepyb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3btfpipkd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ossslyvr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iqcbfqjc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3krkoofvy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3abelluvr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3yvzzdmxr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3pwkeyqqm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hwhinyfj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3cnlicogo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tswsxbti.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3erahkrsb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3jncywofg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gotuzlxu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vpvlwoig.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3wpgfsqzg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vzorynuq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dbycmqcb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3fucgrprc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xotywcrh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3yuiyedyk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lqbrrkrq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3hcnqnthe.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fhxkberq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ursmngqj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3dymmzwng.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zlrrqaah.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3mrxsybkf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cuzvijkn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3remotfpr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mtrzwars.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cfyqayln.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3efznttwt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fkyrusxw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mzjregwa.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sdtjpxju.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3eembaglh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ahnpixbu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fbpbciff.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3mxpxrbhx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3lekfgltv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3uugeipjd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3szhcalnv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3smgtemfn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ohfrrxih.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3unitegsr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jkojnuif.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3dmruihvf.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gczguegg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jemhvpry.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qphovnsm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3wpjoasit.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nnqxyyki.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nxddkcir.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3hfmttgtq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qgdwzaym.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wnzlryoz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hlbfrcja.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vyqimegt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3notxpsph.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3jskleopb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hmafrhyi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wkzawkdf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3dkkhlfos.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hajljhgz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zmjskyvg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pvwnargu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bkccxtmu.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3swqooufk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nuvmjvfx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hncyznre.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3wfpdviza.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3onmbfynq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zdccxpua.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jtyfnfsz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gghcbyoo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jyhgzdip.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xahnmvwh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xergloay.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ieapvbus.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ndfhtugs.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dmusjzzr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3grrieutj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3xjdzkdtl.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3biojvjmc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lxhjakaj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3mkiwjuea.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3qvgprvhq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bxydvqyq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3iikuiowg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xspnysno.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3njchytwc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3kvnjphfn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ibjbubsm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vidqerja.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwjhiadp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3lcpwxgtq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3xrsjthgd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3snfeeyhz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3txkntmsw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3clbwzuaw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gmgvyqps.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3vficdqvh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hcrxstfw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fdbjoygq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3hvlhbygd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3znngqudd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3onqlwcho.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3fkrnwnvs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ulepnbdw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nihqccay.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3abzsiasx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3lgcvlljm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3hspkisvl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3suonhheb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3yeqdqbjg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ppdbmjsc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wzypzxjq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3pxhmuvdu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vqvgussi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ptqlkobq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3trstjywv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jjxlyxlx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3epqetuay.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3aeeuymur.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3yhfaurio.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3osvxepdq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xkxvnvgt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zmhozavr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rtammhpq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ufbchitq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wsrxfhdx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3bfbmrpks.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vuvdwwux.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3uaejdtju.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3slzjortw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3aiiihwoh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3furwahxp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ftddohvo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zukjpapf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pgvuablu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3oaxiewbh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3gwfblqlq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3uegsszdn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3rnyujjdf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3gethahkp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xtkxkbkq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3oasjhmmf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yigjlcav.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3hcisnjom.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ytszwhue.html


<!-- 参考信息 -->