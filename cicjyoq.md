代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsermsfi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fanxiaobao.xyz/Article/details/galfgjwxw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fanxiaobao.xyz/Article/details/gllombggx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoimrldv.sHtML

[D11] 反转数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtaljkip.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvoivjgn.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gnqcjimwu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fanxiaobao.xyz/Article/details/gyzerbhfd.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdtzaopd.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaizaggj.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gtolyttos.sHtML

Ruby: arr.reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gskgkspfs.sHtML

C#:   list.Reverse();
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjilbwls.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfrronir.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fanxiaobao.xyz/Article/details/gaiaezlfj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjktyqhb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhcqzqpa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqdflosl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glexmoxki.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjbokrut.sHtML

Ruby: arr.index(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnxfzfpo.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gndchfoca.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmuwzace.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gkwvrcpqe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofkihxnm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/ghvbstwcf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjzgialn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkfpjerp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fanxiaobao.xyz/Article/details/ginmnfeem.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxwijxti.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhjasfzn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fanxiaobao.xyz/Article/details/goiiaehbf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaobuzzr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/guvkreome.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gelstismv.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/galfvjmco.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gylixhycv.sHtML

Go:   // 手写循环
来源：http://mobile.fanxiaobao.xyz/Article/details/glzjshkxy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gmwryiuyo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrnzggpj.sHtML

[D15] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/giljjymuz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/givnvovca.sHtML

PHP:  array_unique($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gltpzhhvc.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzqnsssu.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfsdgghv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkrjisfh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyntfyrf.sHtML

Ruby: arr.uniq
来源：http://read.share.fanxiaobao.xyz/Article/details/grynhqieu.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawagmunm.sHtML

[D16] 求和与平均值
来源：http://mobile.fanxiaobao.xyz/Article/details/gijsnmnsg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwugyrff.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gcpdzrmau.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gsbginokl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/glndeiwgp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fanxiaobao.xyz/Article/details/gkikpdruc.sHtML

Go:   // 手写循环累加
来源：http://m.share.fanxiaobao.xyz/Article/details/gypjszmbo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkjoopuc.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fanxiaobao.xyz/Article/details/gfnzkpxpk.sHtML

[D17] 最大值与最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gpermowsh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtwddarg.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/glposigls.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glldaloem.sHtML

TS:   Math.max(...arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gkljffrxd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiwckjah.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gixubbckt.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fanxiaobao.xyz/Article/details/gxmlzsoso.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fanxiaobao.xyz/Article/details/glfaacdyg.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fanxiaobao.xyz/Article/details/gcoqjyqag.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fanxiaobao.xyz/Article/details/gtihafoyi.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbcumxpq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqcytenq.sHtML

TS:   nested.flat();
来源：http://m.share.fanxiaobao.xyz/Article/details/gaclnkvrn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gneurujnk.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzzrwnsl.sHtML

Ruby: nested.flatten
来源：http://baike.fanxiaobao.xyz/Article/details/gdxsgimiz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gqhozvfxo.sHtML

[D19] 按字段分组
来源：http://baike.fanxiaobao.xyz/Article/details/geyjqkyrx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmfpyqaw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fanxiaobao.xyz/Article/details/gnxfwinvj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfadtxbol.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/ggmjrtnxn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fanxiaobao.xyz/Article/details/gatnlnvji.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fanxiaobao.xyz/Article/details/gepobtwrk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fanxiaobao.xyz/Article/details/golhwqugb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fanxiaobao.xyz/Article/details/gerzgxrvn.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fanxiaobao.xyz/Article/details/gigikhsbw.sHtML

Py:   Counter(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/glrkfixux.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/grmlnuqve.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fanxiaobao.xyz/Article/details/ghttaaalb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gsncfqqdz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fanxiaobao.xyz/Article/details/gohdiyeum.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fanxiaobao.xyz/Article/details/gzswlrxrn.sHtML

Ruby: arr.tally
来源：http://blog.fanxiaobao.xyz/Article/details/gajfojvyo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fanxiaobao.xyz/Article/details/gnchnihym.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fanxiaobao.xyz/Article/details/gllmrptjb.sHtML

Py:   x in arr
来源：http://m.share.fanxiaobao.xyz/Article/details/grosqxhgr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gymrrmjlk.sHtML

JS:   arr.includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gvvcdokcg.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpbbfiuc.sHtML

Java: list.contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gteospsal.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giusiywjr.sHtML

Ruby: arr.include?(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gzzwjghcd.sHtML

C#:   list.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gfmtmsnpy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqxlnexz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gfdxspzwr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqwhnoke.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvcqufhu.sHtML

TS:   [...arr];
来源：http://3g.fanxiaobao.xyz/Article/details/gteytksdk.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gvsycaidq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfxzfxsd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvhwoium.sHtML

C#:   new List<int>(list);
来源：http://blog.fanxiaobao.xyz/Article/details/gaistmzgx.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxnwzuev.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghozqfrdp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyryalmyo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydnhgmfz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/geofftete.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpsfncns.sHtML

Go:   // 手写循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gthfygkkk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fanxiaobao.xyz/Article/details/gdmjustvb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymauonoy.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gvohggzjn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fanxiaobao.xyz/Article/details/ghempwefh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/giizldlrv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvnkqmmc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gctrbbdit.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkkcctnw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyibdkwb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnrsxudh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fanxiaobao.xyz/Article/details/ghyrwbrpb.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fanxiaobao.xyz/Article/details/gdoubdpqy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmdhzcgu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fanxiaobao.xyz/Article/details/gkllucfsk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gvtntzqkk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgyhtuft.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gbqdnpjzl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fanxiaobao.xyz/Article/details/gogkqkoxe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gplhlvpco.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gxdcbzwfv.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmfhwrzh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjbbbddd.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghplpanxr.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guntafzvr.sHtML

TS:   arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gotuhjxep.sHtML

Java: String.join(", ", list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwwoppor.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fanxiaobao.xyz/Article/details/goshietgr.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghktexbns.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfstxaks.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikugnhlf.sHtML

E. 字符串处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyxqoodo.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvknolftd.sHtML

[E01] 拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyygtmnw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfaikmff.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gowhiqqik.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gsvurgbgi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbccpjdnq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glomgkzlh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fanxiaobao.xyz/Article/details/glvparxtf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcvqfqtp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/ghipoitxq.sHtML

[E02] 重复字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtmkehxp.sHtML

Py:   "ab" * 3
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbuuztpz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fanxiaobao.xyz/Article/details/geghctsuu.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghazsujfr.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhjntdzl.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqyaxumv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gedpkwgrv.sHtML

Ruby: "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/ghgdvaqfc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcydgprwr.sHtML

[E03] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gdizhlwrf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxcxqrju.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibywmaqr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/gouskhdeb.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/guggpaxdg.sHtML

Java: s.substring(1, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/grvlpsudy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fanxiaobao.xyz/Article/details/gccdjocht.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvetvxdq.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gpaeqavds.sHtML

[E04] 查找子串位置
来源：http://blog.fanxiaobao.xyz/Article/details/gcwxamrkz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmzpcnmo.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fanxiaobao.xyz/Article/details/gwqtxcred.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoqyxmva.sHtML

TS:   s.indexOf("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gpovhhvss.sHtML

Java: s.indexOf("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhczrfkf.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fanxiaobao.xyz/Article/details/gfsqdxufh.sHtML

Ruby: s.index("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskztcqvi.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyafyhkol.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fanxiaobao.xyz/Article/details/gvsybtiya.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gojcybhuf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyexztnw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gwtilxwci.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gsmwtejun.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fanxiaobao.xyz/Article/details/gurnewkwa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fanxiaobao.xyz/Article/details/gaetgafjj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gymzyrsnx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fanxiaobao.xyz/Article/details/gomdpfmsi.sHtML

[E06] 替换子串
来源：http://blog.fanxiaobao.xyz/Article/details/gjurziysb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fanxiaobao.xyz/Article/details/ggdwpdhqw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gvcddqiay.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gddamjmrh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/geozbkltf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysrirtwe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/guqdftrzn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmhhfsrf.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/giwfrokpl.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnwjhcmu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fanxiaobao.xyz/Article/details/gsrchkwyt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/giozhqpja.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gittnhncy.sHtML

TS:   s.split(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqvpekck.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fanxiaobao.xyz/Article/details/gdgppgojy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/grkxxanaf.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fanxiaobao.xyz/Article/details/gckiwbuve.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fanxiaobao.xyz/Article/details/gauelwpxc.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorolkidz.sHtML

Py:   ",".join(items)
来源：http://blog.fanxiaobao.xyz/Article/details/gojeebsak.sHtML

PHP:  implode(",", $items);
来源：http://3g.fanxiaobao.xyz/Article/details/grqbtxygq.sHtML

JS:   items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpnwelnt.sHtML

TS:   items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfygxryf.sHtML

Java: String.join(",", items)
来源：http://wap.fanxiaobao.xyz/Article/details/gnolhefpu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoaxlhcm.sHtML

Ruby: items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gwbvisxch.sHtML

C#:   string.Join(",", items)
来源：http://wap.fanxiaobao.xyz/Article/details/gdqbrebai.sHtML

[E09] 去除所有空白字符
来源：http://baike.fanxiaobao.xyz/Article/details/gxlbsniwt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkzznwlq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsompxfne.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fanxiaobao.xyz/Article/details/glbxeedno.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gjtwkglqr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gptaorixp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gubpclorv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gzelfbrwr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gybmqhjis.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fanxiaobao.xyz/Article/details/gxrudczol.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gcksbjkqf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvadcmnkg.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/guezbveak.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gulgzcsrp.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gxeognhsa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilajotiq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvitifzsh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcnvtoig.sHtML

[E11] 反转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxraqfrmx.sHtML

Py:   s[::-1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gliqosvlh.sHtML

PHP:  strrev($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneoxwesy.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhlirlbw.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gctxnavjy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbwleias.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/gpvvcbicm.sHtML

Ruby: s.reverse
来源：http://blog.fanxiaobao.xyz/Article/details/ggbtqsvuz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxhbbfma.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyfkivoj.sHtML

Py:   s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvcuyazv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfznuobk.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqmqcilo.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvfhdhhw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goumdbvxo.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohwrzxbx.sHtML

Ruby: s.count("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezkdaqqt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjtjtevz.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonogkqrc.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeqofywp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gasxkrhhn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsijiejj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/gbpzgzbth.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gjlrkykhn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiltmcro.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fanxiaobao.xyz/Article/details/gqgcwmnwh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqogwxzax.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fanxiaobao.xyz/Article/details/gjvbidxju.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fanxiaobao.xyz/Article/details/gikprlpvl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gewiaymeh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrrwnqqp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groybrwhl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxtgqlol.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fanxiaobao.xyz/Article/details/grnfeonul.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fanxiaobao.xyz/Article/details/giphcztyl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/ginbthlqk.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fanxiaobao.xyz/Article/details/ghetayrlk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjogovbqd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fanxiaobao.xyz/Article/details/grlvgmnjo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdproftmd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeavxlba.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtqcnzex.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsoiarig.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gonotbwey.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomeoznad.sHtML

[E16] 数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gamjrirrc.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkgmukra.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadlihtjo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fanxiaobao.xyz/Article/details/gaagsmhjj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcujacxg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkecixmji.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fanxiaobao.xyz/Article/details/gfkgtzafr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqctefdox.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqqaokuq.sHtML

[E17] 首字母大写
来源：http://blog.fanxiaobao.xyz/Article/details/grrfkjpit.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgwphaau.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gjnvlbtzr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/giqyaxkmf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpamdxeqa.sHtML


<!-- 参考信息 -->