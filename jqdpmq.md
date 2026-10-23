代发 wailian999

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3isjnynca.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3davyrmlq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vyfxwugx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3bjyjuyrq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3peptyyeb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3lzgqkcfn.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3brscnydy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ssxuzxvu.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ephadevp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3wsmdhpqq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ssahukqj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dabkexor.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ejtzywpk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3frxbdksu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3yawltfhb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mehyutuz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tmkbpypj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3zmywexta.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3bpylvtia.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ozmvbdhq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3kzmlbvus.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ukwvwpzf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uebmsbwq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jwglkypd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zlywassu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3mcrgymoo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nnwqhlwu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3pbamvglh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bkdtlbci.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ftdnuesr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3kaolvpnj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3leryulmx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ykwqoxtc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xiixchzj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ygjjsjki.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3txhcahxs.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3lxnaslwt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ebfnwvxm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3lnqpexho.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3otpbqhpj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lleasafl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3gzctdoag.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ilhehknp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3aqygqlse.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3gldxelkm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3swwyabkl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nkicyexk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zbxjvkui.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3btnlfeaq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xeabvemg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3pzvsecfk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3pirtnahz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3eciirkfc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3oiodqifl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hcelgndm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mjrkbiqj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3oqffgciq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3fdubkjdh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ajcyactb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lusxjhwl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3bqgrbzpi.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3xytdbpxe.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3dhgwenhi.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3jlpjzvmm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ntvhnisc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3qfyfoytz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3rtsllktm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3iwychqtr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3leazpsdt.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vvapqntp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3bbxbstky.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3atykhzpk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3pvwcbtkp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3xcsittok.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3nlirdzsk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3qwhhegrh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ifqiryli.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3uyzyzula.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3saouedfb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3phxgeazk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3qzhbvzof.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3qzgywels.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ptkepocw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3sawmettu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3caeumefo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vjujgcwq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3sowirmbx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3eidiqxwx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3pewbufhv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ljlsjhgr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3jovqzcrh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3bljhazog.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dpnpfqis.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uumwktjo.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gjqogtsi.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zlamvzsi.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iwqtrpur.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3snyapkoj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sodpatzg.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3sgbknfin.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3jocgenqp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mgjgpctu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ktjjvxlj.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3zumfygnu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3oaylzupw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3kfceiazf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ntsrhsxa.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rasrxasn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3supjgkin.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lqmgdkbc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3hazmlmcs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ugcbyxto.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3djrylxfd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3fgzddfxz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3cuvzrwpb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3emkpnheg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3hvxxpcfh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3uwhsqeyq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jmibvdsh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fegqitus.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3krxprodr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gayanetq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qtqrtwoz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3rjdbfmzk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ubccucue.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ptpxnxyc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3xrjxctkr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wwqspdeu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rrdfwhqn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3cinsnqgz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3gjtfantn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zqdxhjoh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3xdhwrgjg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vmctkscp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lhuweazy.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3wbkxnwvp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tzmpwhpc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3difkckgr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gklelvwg.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dpcbvxps.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tlorqwnf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wtppivfn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zeggauyv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3njoolrpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zppokwpq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3cnbsozyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ermuyvep.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aphrdupo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3bfxfxtba.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kndlopea.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tjcfdihc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3skiisdia.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3nsnbwpbm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3gvulbksd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3fczadols.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3toyfqpbj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uxbhqgxk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3rulyzbtw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qfjkeqka.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oqamutmf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mffnohhi.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vonsybgg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fxytlpsz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3hrjuavix.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tytfvtbj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3knjtxblv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3oconaiin.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3aacvnrru.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qdcqrebo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wkyhducn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kwpzeqhq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wcpmkxge.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3vzdinqon.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ilnlwdht.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jmgirbqo.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3trpifobt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3jnbcubhz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3jvbxgvuc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3laymicpo.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3osktktph.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3pjwsvcnb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kynpsenj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mixhyslx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3puzkkhvk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3blpsdvsh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3acikijxd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wzgndmex.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aivhzrad.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vjimbmiy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3wilsluxp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3rmjpczpz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xnemooqc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3hxqbehsr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bsaqyhnt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jypsofig.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eqgbeyoq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cvrbxyxf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bxnxrzzu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ueopjivw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gmmjswvv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3swzxagrz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3iqgeaime.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3eynhbfcq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fjdgsyho.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3nvlcnvta.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nfbyvjar.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3kygtulna.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3xynubuzn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3lemsgpxt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3mwjuiwlu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3smiqucvm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3fddfdwif.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3efygrycv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xyafzjiw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pjixmpys.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3snfpltvo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3vtxbdklj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jtaktucs.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nejbxfhu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ooxgrnbu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3hfbqhuun.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fpryalda.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gzrdcwmk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kqqhncsf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hdjiqogt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3hsmtdmgn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kdqadquw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kehcohtz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3mubrrnsr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ygmsgpmh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3dusslwxl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vpnalwuf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ezfvheuk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3idzvrqqd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uawuscde.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zpvksvim.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3yepbcvei.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3upuzyyfq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jodbjjrm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hnyjahsk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sjdwierk.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mwexlzfl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dgndvvzc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dmgxzjpf.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3yzgkzxqo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wvuhjfkb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vfhcabdg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mqsudtjy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ehvuoxwk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fnsfuimm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qmmgltze.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3pqvjzwii.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3bilshlax.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fvmfhnpl.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lgpuinpr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vbhaecld.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3zryoywei.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3bqoyfsvj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kwltnftk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dtrtssir.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ahhnxmpa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3mvbrerqx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3dqhtmrjs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rpbwhpst.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3brcqfdar.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ucsozhbx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qkszpwwk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3udwminbx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3awcbmbph.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bbretjlu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3izewuzje.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3gdpsxtxw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qjunxbpg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3kwdejutt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aritcisq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qwertmbx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3cacihnft.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wpctuutj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3vedoocdp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3avufohne.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3wajinvpd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pznqrmng.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ujcyhvjt.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3qspwjgqf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3dgxpkwij.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3iawhftmd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bjjwkalh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3zjsqlpzc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3sjzvthjl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3stugkbtd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3oynghlpf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3vmgafsjs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3tdjflyqt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3walqzzry.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ntjembld.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3evfayzvo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wdxdvbkg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rzarectc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hahwzkof.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3yfbfomai.html


<!-- 参考信息 -->