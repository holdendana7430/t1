代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3tjftizlu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3wbcjraxj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xxfdkuvv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3cfuzgfuq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xjqkrexo.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jtyqrpqa.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3avbriuoj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wutmbhmt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fpumclvb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3vglpscas.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3iyjranpt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3hagdpurp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3luexitne.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pdmdktlo.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3cifvmfcc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3byqddeus.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3jhgzuvbh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ssgnqead.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mblqxwbv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3daetlmyh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3jmtpnvnr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3oezhdyzr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3byevidhg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3xltjygkc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3wlxflfyw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3bguodhcd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3teqvaebx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3hdfoatzg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ieltchqb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3edmvvnac.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3kunqciyf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3zgjkyxkx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3auzwbekq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ftwcdqfc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rfmhohgy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3bjdsgdhk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rdhxmpzh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dejzltqu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3vsfbvele.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fdantqzy.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dwwzxpbt.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3mucvdpph.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ubhsnghm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rlntpkdl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3hmqommnx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lefwywbs.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ygsevohx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3kexqdozf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3gwcmggua.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3otzazomo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hegkxfai.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3vjwskdec.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3drxsndtq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dbnlgyhe.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hyiqnmzs.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ncejnwnj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ngnjpyxf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ycsotbef.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kxjusoxv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pihwbdrx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3uvamcvjl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wzczxdls.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kjcbkmmq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3koisatyp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nkjvfynx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3wbdclllk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ynprrmfk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3mrxmlnwq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3jzuhxfnz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3iwhwcqla.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aecbaspy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3esxyncqz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ebdftknv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3oxdpxgcn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3hbeophif.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3upizopbs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ryploonq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ppgkbvlo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jblaokey.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wkawqmeh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3bqyflnpx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cofwdtmf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3zlirxbnq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kpyohrwv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ovnkreqw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3wutgduki.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3pdofrhlz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3eswtqaij.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3zthpowpv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3buxrwnbe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3fqwboynv.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3wwqlhmib.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zioesgje.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3iawibzqn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ejgtaotf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nrfutfjg.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ztrbjfmx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yjnzqtwz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ypdshxcs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qaqwbxyv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dmvbckir.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3kzeimhic.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3jygyvpmt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3xvbcpbwp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3qndquibb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vtuyvhst.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pyabbawd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wiwmryrn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fyiuqwqn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3crgfculj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ztddyjin.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3leqwlaim.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3oaljojdy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3uocfikmk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3tufkyvuz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3wryhwnbj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3rbclmbfr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3plgttubi.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3enuzzqlg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3edrmrptq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ykgzdzjs.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jfqxxama.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ymmdtmra.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3xpmtfxud.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3wrhfvoqk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3oiierswx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3usobkhsg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3mmlxscdm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3kkvwwipx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wtziqfon.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ampfjapk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3yrtsmtai.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3wqdvhzzv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3eqdiyqcz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3nrtjtfhz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fyszekki.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jdxstjqx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ibzjzihr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tjabtmpf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3hdytokij.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ayfgjjfe.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3nltfxyoz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gtqfvamz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xonebdyt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3crowgxln.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sksupzlb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ehntyobx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3axzrglbp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3okotyzkk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3lqswrbiz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3fmaphgpd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3kwvnvxwm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3itmnqfnv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dqbhgmse.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3lrjcsdcm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3sfvaaeqn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3hvctkduv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3exbkcsgz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vdoanpie.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hozyarxz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3fcyxqwik.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zbcbalpl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jmpochxp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ttvlgsmg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3trzddyly.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3efgaakez.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ritjstpb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3nbzbaqyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arrkspbr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3jmxquziz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzeywkoj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pfthzgvj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3sevaegkz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yofyzkvb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fpdbqpky.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bvtehmbl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3zabekdjw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3hanwzelw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3dgukloei.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hopqcowy.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3momnqhua.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hfnhtmfa.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3exmtguxo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yqduocsf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3crmmqdjz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ioxqmxyy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wvumiimz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3sqtzfloj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hgaupcos.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qoidnbgh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3dgtiykrb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vqzegnnd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oskweqhl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vovyykkp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rnvzybyz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3occyzdwz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3dfuuavia.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3cpbqilgp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3lzxjtepl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3unvuipzs.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3hqimnjsu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3yssddzvl.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uceutpsx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mqmkouzi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3hjpzccat.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fmhshxdk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zmoftlgr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3uqkivqqp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3jcrfzvoj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3nubrqtvy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zcnxsudb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dgclgvww.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hvswbtud.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3xlndokaw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dalwezhv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3siyuqitg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3wfcpyunm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hdtxxbmv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fufvujtn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iufpuppc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tqttilgw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3romzyxhn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ovitguxt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mionckog.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3msvwocje.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3kxtyxcut.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3knvrcjjk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ogcygscu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3bwiqonjq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ysxopccg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3suqflhpr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bbigpjtk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3qnmwpvkb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3rgnxomjv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3gqxlzqxo.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3sbyfnsxr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3agxhovnv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gjxjsnqr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fyftbynx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zkrikadg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ewyrhalr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rnbkvlrs.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3cpjiihxd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3epnggyqn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3znbgufwo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3soxmhocj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3oizeuadx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hktpwtxo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fwzznaea.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3cjbeqhpe.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3fbfimqpy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ecwmcmch.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3iiqusejf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3poseymqn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3afkwemzi.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3frksanta.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qvqylmiy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3uupnnxvo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3njioxdsm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ivulraut.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3emrpkhkb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3loeaelwx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bqsniutz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bgrgntsa.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qaycpfyy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3khsvqjaj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vkdjcboc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3iwjhsnuo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fcvlictt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nykliyfo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3xlyfwpec.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vgujnonm.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lxtdammq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3trtgabqm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qhasehqb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3qvujbnhq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3qhfidsvg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hmpxldcl.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3aokhjied.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3gkoobedg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3dqqzzoei.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3prdnesjs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3chroyhjk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhmenkuu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3olwodfse.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3adaunqen.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3bhagkiwf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yzeakjqb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3tfzwclgr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ifqlevqm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zegoazby.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3rqkfyfks.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3uyncmzep.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lwifooul.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3gshjvtso.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3qvpmldmy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3chvgkgbd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3kjxlduhu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3cpxajgoi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3yuzckcni.html


<!-- 参考信息 -->