代发 wailian999

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3smmpnzkg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3kxdghrjy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3usqyyone.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3scedycue.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ervrdveu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3fclcgenp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3viokjzbe.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ygvrldxg.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3hnggwrap.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3mpxinkbx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3dprmkwcr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vgzfziwq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3frrcshxp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kwlodeni.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3dsbnhqgf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yeuplmmj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3zatcswcq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3rdvgqagg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3pqzjbski.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3owzqfkqx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xkctduhq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fxrfacwd.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pnvrhzlb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3myxmikoc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ogrcsvlb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3hjuyauza.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lxkulbff.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3rqxnovbm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3pqsnlibk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pppptqwj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lttseahv.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pwiddjwk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zjctxtxg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nbdgubbh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vauifusj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wlrtzsnh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3imjwbwcb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3atdqizqc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hdedtiap.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qkaaryjd.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3llxxtoce.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3huxmomme.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3awfaprin.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3feezwbpt.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3dmaqvhae.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3foywzfdf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ykupcxso.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ubukcjgc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qbjrtlio.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3tuvzdpkf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3eqhcxdlr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ixqnlnsn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qdpgjual.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3rqsjdict.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3qkrmwyct.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iveqmgag.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gxixntes.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wiqyivur.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3rughxjny.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ahutkqdl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ekhssddo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3bruvbzqy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3egrejboq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3yyqxdfhn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3kgnbowni.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ywvfjdhc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3tinhdztw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3hwgmaxek.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zvcsttqi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3abeexwjv.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3kmoqdqny.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wsonmbxt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3zuwuwzis.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lidxxqdk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3wkapatwa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3rgqthkna.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3dzuxrgdy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3zbtrwdxr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3eshacgrg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3aurgqrqf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3idavrtak.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3foyexvbd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3navfkmax.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wzrevwog.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zmyvazmm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pelnrumb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ietfbvzl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3nprobqwy.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3xmgefavm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3cvjmgcvd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ejeorzrj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hpwldpbb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3yonwnxuh.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qwqpmddq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bfayouvd.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3htefisai.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bscneebf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3cjgjbdza.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rzueahnv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3etdyigtw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3biugxxqx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3kdnzsegh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rrqidkkl.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3hadcxzus.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3bfteevgk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3cmtirgjo.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3nkklsbaw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xoaeouvv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3cihgedtx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nqeqqaum.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gglucbdm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kncxbedf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sqlthfef.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3gzkxguqx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qrjlalaa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3sbtrmsud.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3entafylu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3tvmietpz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3tmbvivxk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3gawudiht.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pkritpet.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dadavlyx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pfjbtiea.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3asljipxv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3nyjpwgbk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3wzpcypyi.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ucqzhtwp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3pzmwckuj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3fqycmyty.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zlyhgtiw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3lzstyyao.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nnrvmqdn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gpwlijhr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3cswcsqqs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zroptihj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mievyxrw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3klbzipei.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pgqxqnei.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3avxaynlb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wlqvouqc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3msochdil.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3lpxqkese.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3guzbyrpo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qfcwlphu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqzyhcji.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3womehosh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aubqayhu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bodlviqf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3clpsquel.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eihgmmrj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ndeiqskd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ojnkykkc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3qjadqvnr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3cbuubryd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3jfjqmohf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xxgyxajg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3falgrhxf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ygpxlgma.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pgiepamv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jugozwen.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zrcbawuu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hkqrmjgj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nabforoh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3uoxscezv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zayelect.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3yiwypihe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3sceixrss.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3npzjzrtz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cqxqilko.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uwkpxgrd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3paqaaetz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dljewmzq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qwxhyavx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yuzpyhpx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3beetvvpt.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kxqgtqpg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3phhdawna.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3jahwmhdp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hczqgpmh.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dvkteewp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ktpsfkvh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vyimibfn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hbjlhhkf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3gacjavxf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3kxygenry.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3jjziqcgg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tjdolfgb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3cbeciqpa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nwzgrpco.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ptvhguat.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wqqkoplw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ujnujibf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3mviqjxyj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3golzcshv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3cvdxewyp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pvrbqcyo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bwskwwwq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hgpplagi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tqvemoej.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yqwqievr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3simfkasv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3amhaznol.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3uuaevjlu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jlocthrb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3nvyhzmeo.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3egccxpre.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dzdiykcs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kzoadjtt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3uvpkrobp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3gfcjabig.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3lyxnudmr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3rxjcdzrr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3mvjuzunr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cbtvczfx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mduwkymy.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mxkcfrpx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3xoirfmnh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cupzfunq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lqsoudsg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3jnmedaho.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ihklpfss.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3eovtmslz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rbgvzvch.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3samidxow.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ryxlwhpn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3obszroiz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rqsuishn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xahtfwce.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3jnmxbzbd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fubebdhm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3nazinxxk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ulzbnikp.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3burliefo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rdinwgkc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wlhvhjfi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3prvlnasm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3dngjwocx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ovmrhazg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xnyzzuuk.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zzcglpqx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3okvlzonw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3osjyaezz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3fstwella.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3akhwqsow.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tgbzcovc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3eyagkreh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3flzpiujm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bgdxnnbo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3uctvhfzz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3sadoputq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tzrvcbdd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3adfgvakl.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3zokdvyuh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jbwkivbc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3fumaqwnq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3rlfdvgkl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ureggsyl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mnyatjmm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3klesuxii.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3implbqyc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3oxdqztld.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3hjqdorii.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3brjvgibx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3aikakway.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3mydnvwsw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3bskjafgj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jxzjnbrm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3pzlrvatb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3tufhhuhp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fubqrvlu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3svdfsqzu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3acwxgrme.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xhkavwpm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3btcegvyp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3vkgqxyys.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qziosqci.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3linumool.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qitkapwi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3jqjhqjii.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3uklwogcx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3orsysdzd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wcegbzby.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3muackolh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3obzepnvw.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3yyfvhqog.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cedjinqq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dkipryfi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3cxvweytz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3azxxodql.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3iahivyel.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3yxkjxozc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wxpzoyav.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3heairyfm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3akbrdieh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3sfpitczb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yqgosoji.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3mpfmdlnv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3tjcqwogb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jrugmztw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ywtvcpim.html


<!-- 参考信息 -->