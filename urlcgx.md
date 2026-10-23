代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fetbeyna.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3irmlbtcf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3rpsxvarv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3gmxewboa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3jikjarpo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3myolgsqo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qvfmwgcg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qydmqsjj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3gvqhhilk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3gggicobs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ffhwigbm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3cjsahgle.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3pljrgcaq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3opdtqivy.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hixgyxnc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3pctmpyzq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3fxisziwy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3zxpdmfaw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3bikpilrc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3mvshprvz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vtuuajsp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3wtytxpxx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3alocyamj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ljcfivmx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3oapjelzt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vtibenfp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3cdpuezso.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nzwacort.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3vzjnceoe.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fpyiaxfn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3lofmbhhq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ylcucxww.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3depdfomu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mqddxqie.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3izhaubzf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3nyatwdeb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3utkputgf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3igzuwagl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3itoraogx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3cxvbmqdr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3syoyasxu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vluqkchu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gqcwjfgu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jzmbyhvq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3pdvmiqdy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3myumdfde.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3aoqsrbhx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bbstwtej.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ckgzdrcb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3poxxvmrp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hjopfaas.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3revbjlsz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cjtowkcj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ownxvxzn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ijnmgnkj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3uhtihiog.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3luwufrsd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3zvkjslox.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ykbcwikr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3chmqsoho.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pfcudeuo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yxdqmncc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vimxsfmr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3twirpkxk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ikrkmksi.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3mtdyywsa.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dfqryxzp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lemuicph.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3mhxwaaec.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3jrdiatlt.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vuqppjhs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zcccfrpr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zwcwrkdv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3vdgjhvwa.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3frewfpjj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3vantpmjs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3sffwxsay.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3kfwqzlai.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wgfhauyr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3duzzytor.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eqnbivao.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3yxdznyxj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ileevjoi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yemgwoxo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3tojemftf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tyjcdksy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3paqkpsxq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3vbhyxfgf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ejzpreuk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3kciheens.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3wdfxokfy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3gvjtxhfa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3sgnkkqwz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ufkbbrkw.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3aougtyxq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nwpdxixf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vwktdwcl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3eztiogpe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3uxvkxvfn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3fpaosxrh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3gcndosbe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3fuvmiqje.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3roptoocp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3uxsizwiw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3wosikuip.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wuyvkily.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwsawwye.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wlhsvfhs.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hpqtjmax.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbdcshus.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3etrssyem.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ygspbhxy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ziyqofqk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3aijztyhu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kgdyagqz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3pdgypzha.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ghkylwzc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3kfvzqlte.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3wxpebrvq.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3styjxuly.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3kduzyenm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hnvdvhgy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3aaubkjat.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aemffvvi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gyzlnhvj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3fwulezay.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3htuygurr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3tcrzinkq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3cuauvnzp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3btszgbdg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3fntbjgeu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nrhfdomu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ulhdncbf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jxutyiih.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jfcxbicy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3uakvqwkk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3liawqvri.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3fexqstyz.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3qdfwhshm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3nbuxzrfa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xbgmaksc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3qjsaswnd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ofsepqhc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3oxvsejuk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3fmxhfnjc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3hornxrhn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bzwalhtn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gjyvhhzg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ahphtitp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ppvbuaxn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zqgtzshw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3emldnhzz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3eapabddk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3yapjvajo.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yyxnqkbz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wzyhxcfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ptxqbmpp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3incgsacg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtxjtkdv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bltgpmym.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ztshngsh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3cwmsivpl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mkmqjbmj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tsnighvv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3xhefpzms.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aifcxssz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3svgudyik.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ufkmexzi.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bxzzejtl.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ndpochcn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ngrwuwtx.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oomaeynk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wurfcljt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3luqplqwi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3htfmkmut.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dkbxclbp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3uqpciews.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jjckbbgf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3thndzjsa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3anrgkhqp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ocsaacnk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3obdjeerd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dxivuyul.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gxlzxoxn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3yzhmcsfa.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pflfadub.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3hgbtdhhp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cujihxwi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3slkujrps.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3plmxnzwe.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tzeqckfm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3drltgulg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3asmtjcsb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wlezggzl.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3katiyxtd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ykrvxxum.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gpghqtol.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3sxjngzkv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3atgfkkxe.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nuhfhepb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3htlmbvqn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3orkuuyns.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cupuugwi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lwjtaavc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ynhvbguz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kitxhgfo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3exerwxao.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dlwjpoph.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3runobhax.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ppwvxxwe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptqcudsh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3icozzqtq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kpuxmqgt.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3pmdswfvv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3nzmpdray.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pdtqvpse.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3veoehimd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3zjqwalpl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ysuszrom.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3cmptpdpb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3fveffmrq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3xbqekptw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3acuhxjgd.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3qfoeqhat.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3flglncbq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gqkorpue.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wemtequg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3eimdhwuc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3cyfnidvr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uaejbbnb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3cgyvmxqb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3gexoeokf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mqqtqclh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3iuoxbcrb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3syqtzbcj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uvquufbr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gxglgbdc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ysahaumn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wfawobtc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xrdqfrrb.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ktdvfpor.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xhhjhhtv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3raipdytg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wwuzgsgi.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ijyorwwd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yuqadplg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nsobbobg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qlskzbrt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3xulrhelq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zohqxhsp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vfdsdhwk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ehgrzdzo.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cvsywdje.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bjdgthcv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3swlequuv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vjoesoyx.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lzefbhvr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dqebuxrf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3rjrjlgqg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xvtquaoa.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lghszpuz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ayoybzog.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3idmpdvjs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3evmsyiut.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zhqgzkck.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fodlhzar.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3vunnjgnx.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qabowesb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3timsfxxm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3tippahjj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lmxpmvmm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3obkxhvvm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgqfuzdg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3gxayudba.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3vnuwfahy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfnhavtr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3hkbompwc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3frkpdfmy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3weoofici.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3yifonguv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tbhvgruk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xwdhofzs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3pswstjex.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3cewykwzs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qiegupxg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3pvfxymwx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3yfmoeizs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ljeqsixu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3emqiamfw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bakzilak.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3siexqixc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mojknult.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3jhjbvplb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sujrdryz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wergynli.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gevmeraf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3jjqiwoaf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ztvzmzaz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3tnxcmcbh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xgexbxtv.html


<!-- 参考信息 -->