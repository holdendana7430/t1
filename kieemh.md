代发 wailian999

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3punpjrwx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3wgczeqct.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3oeisaloj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ltenwpht.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ucfmvyje.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bfvsclbf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3jeoenlei.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3awnqfgnf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bjwtkihi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dfqqtvac.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rgfzzwqr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3iraysbyx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3aliuwrgx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3raikukls.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3okafryek.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3vagpcnhp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ixqgufhg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3coeejydc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3skzbflum.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3adbjhtek.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3abcpzdwl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3xhrwdhrh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3wuqphibj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ickvjpma.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3uhsbahvo.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3dkvffdqe.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3fwqgxabc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oggwntfb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vkrgiavt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vtejmnvp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3yuwnioqz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzyfzdxj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3cksuizza.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3milhtily.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ekjtcpna.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ihtocldv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3sseahmzd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jtzczilw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jwckujpb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3trvcnmmr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3rznbfqdu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3mzoevcgv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xlnspthr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3kllkujpw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ubjhwdtp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3caiymrgh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3kushgkeu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rnzdtvnw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3kxfvhfno.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ucqmuznd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gchftchz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mppjdgjv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zgwqopip.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qgbvdhla.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sbxnlmbc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tkbqnttc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3znlwqccz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3isofdsoy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ihuxhfxu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3cnjrlbnr.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3pagbbwml.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3agopzvqa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nhyaudnm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kiqmtbqt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kvjzevxq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gnxhuzxs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3eeuxwnbs.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3rnpzwcoq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3njsrxqdf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3hxbowhqy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qldssmro.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nbjbgsdi.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gjwfxaxq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gkwghtfk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3qxnhchfs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3zvdrggvd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tbhghhib.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ozzqfnoy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3nfsvcjpt.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3logtbien.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3beqjujru.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3xeldchrp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3kjmerqaz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3wqnoazaw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pjdtzluo.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3tbmrofve.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3cpqbmcuf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lcqzozet.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3puvlzgml.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3egzuiiug.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3jfqythwk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3fiqsqraz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3szqsaynj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3msvsfdqr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ywqpnhjm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3fkuhonlr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3refxlxxj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3quqzsnnw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kxygrrqz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3hlnbinou.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mgekuxug.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3swjvfegq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3uengenai.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3qmbfjeyz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3iivhmctm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3pxdrnmnh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3bagoevll.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pfijzdqo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ymhrrxry.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ylzuzmiu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jubqqlsm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dcukbuzt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3epkpizjp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gzytpoll.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dvrnzpnm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3biseowop.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3iuxhejjz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3vyspwymx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qhkuwqpo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3agiilswy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dqpjgyvx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lofuznks.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xrvutmna.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mtowjxuu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ejtljjbr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3pfkwmmrt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kmspvgmc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bvehlsqh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dxhwuqyj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3zpkxshww.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3onqhjswy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3denewims.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3wrteuyil.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ikmyazpn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3fkvfxusv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vjzciepn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3gdnqgaqw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qonvjguw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3uttunsxo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3hachauqk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3wazetehd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3nfhmczav.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3bxynpavp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wsdmzrmz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3jsbzvldn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3qbjvpgit.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3crtpxfdo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhsqystk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gityiien.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3joihdhlc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sijarfpt.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3fkyjgtxd.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3dgrymizc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ihblxzix.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pxyxvayh.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yqtwkdfc.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3kuundcnm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3slyghilj.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vcqilxws.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jjfimqak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idyxvrkh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3wtdyvazo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdjrbghe.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hsuzuplj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3bhqzdiiw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3nleasxoe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jymjmodw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sbkynggo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3jekmtgya.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3udldqodf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3yalsuzzd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wrqnqzry.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xqlrnrmd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3cudqzwtw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3fdqldyso.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gzeiksrr.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3sjkyjsfd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dodwpuhg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nvfqjnkt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3lbunwoms.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zcxlraie.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hbuuwdlu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3oomatycq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zixayeap.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qmismwbi.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fvyhlxeh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iufszleb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3pwzvngzi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3uwkfydxo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3mnqilupn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3xltitboh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3emogryno.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3loqodmbt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3blgncarb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3taviovuq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jlxuoyhu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3pjgaigol.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wwvjxsck.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nmhtnmvg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3mvfebxed.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ercrnwzw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3khcoskly.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3climqnhj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gvlagmkx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fztsqdup.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ewvzdfgr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3cbacmuag.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ijfospvv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3zufnupbb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sdoowjtk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eqympmsx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3slfdizye.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cwnakphg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lwyiupiy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jaovczxd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sojfhxod.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cuonqbbi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3hdncjlnt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3tvhqfgbz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mlmfglzq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3eluxcufz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rjlvegfs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3wmgchnvp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ttgvchfu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3iofshzsh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3epkaoqkc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ayhshjxg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ulamozbl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ffsslpeb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3anjdpkse.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kifavpcq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ftgcdxze.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3rapzvner.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hhsquedd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wzlyftbp.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3amifkwrl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ifshmapj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3dzdkfghm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rszlwhgg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jxdsbdes.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3fkxtqvot.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3utsumzkt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fyadkvjc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ddvwsvtj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3kgxqewyu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ncpkxfxd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ztlapbmv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wuprbjfb.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vhtbkfgs.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fsuuixrz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xztoiatr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kgbajnkn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3xfqdnvtg.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ydnadewr.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3waursjev.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uufxzppx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3reyizkhq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vftdrqdi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ypjtnnmh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vczznqkq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nknoqmwe.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wkdsboiq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3mzdgrqsn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tjjsttdu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3pfmrwvqs.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vxzdjfjo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3eylfilhv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3uolhdapy.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3flrgysad.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lsdocxks.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3bwaeygdc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3pamjsmbf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3vdeeqcmr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3jwrjbdby.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vkoimkhm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ffvskhdh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ptzgsxds.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jdfffisg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3nohdilvy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3elcrlzeq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3dmtnqobv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3lumethty.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3rhnoyzun.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3evrntveu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3etvwrkdr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lxgrjfjm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3sgrkzxmq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3iqnjcazl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lepmgxho.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xbkmdzuq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qwpncdkz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bffmxugo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qsoalhzu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lxsyntnx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3djewdwru.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3rjdxkxsi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hwifwrrx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3upkmejpw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3phycxlzg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3dqmcesyv.html


<!-- 参考信息 -->