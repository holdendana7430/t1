代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gneejgaji.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gduhayewj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gtofwrwep.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gbhtrehva.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gihilauya.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gayhngnue.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gxseectdv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gtrhoxydg.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/ggevmtrjd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/grsdxwdzy.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/godgllhuj.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gfsslablu.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/giankfgon.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gsfmeqtml.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/ghmkboyqz.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gpclpqsvv.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gqdpdtgyw.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gvavriwoc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gaxltlmbk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/guefutvaf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/ghbeihgqp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gwoffemoc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gvmiefkkh.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gpgkacqhj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/goerbntyw.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gvfidrlva.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gkbxpnigr.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gticemhov.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/guprbpnif.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/ghofixife.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gqgnixyvg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gasdwatln.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/guczdtsed.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gmwuynmyz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gbzamdkse.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/giwlhjhpo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gpanrgdln.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/ggchyxmaq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gazkrczhg.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gpgzcwyom.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gvpxuafqk.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gtwcisdyp.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/ggrdwtblc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gprayvsue.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/glkbtjllp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gjwuctvye.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/ghtjbtwhx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gighquvrh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/grpojbmps.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gjxberxsf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gxsqcvwdn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/glmtoasua.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gwekycbix.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gdfkqpfzl.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gtbchbizl.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gioduxxel.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gicdywwev.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gbkjnqfcw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/gajnkovbf.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gabsfaxwr.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gptjlwqcf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gkzrobttb.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gyxowpytc.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gnpzuqmeh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gvvnyurqt.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/glersuflp.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gxbpxezqd.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gldiomdnx.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gzsignelk.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/guryjwtvt.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gocfphuew.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/guupeiars.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gkqnvjycw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gwkjbxbsm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gwqkkasyy.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gcgvmhnyf.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gvqeetmmi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gotyvfrxn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gtpedonyb.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/ganpxawkt.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gaxwoktgm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gicyvxrib.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/giociobil.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/grhtdljvh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gwqucwwqf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gqsqefuax.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gtrbltnne.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gbssypsfy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gqodbsycp.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gkcgcdvyk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gmsuzrjvl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/genvdbkkv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gkzbanagw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gbjhlillp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gayhzdelp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gncfunfzt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gwuvefymi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gdnmiowpz.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gnvhuwqcg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gajyrfgps.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gvpouzysg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gpyfryuqb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gryouojqx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/grlechmnj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gcweuztrz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gumqedbxw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gachrcrbk.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gshistzzr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/grsvjwdfs.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/guunxbnrs.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gkrqimmxz.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gnzijxmfp.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gclwxsukz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gmcmhrkhv.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gpvglcvyf.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gkednebsh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqxajbiav.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gnykwdueq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcmhfwawy.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gomxhttoy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gsshaumap.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gklitxcgp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gqlxeuaxe.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gvrqsrsue.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gdvfcnmqw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gjwsyzkcr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gjnxnautu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/grvnclgrj.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gvjxydpnf.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gabxztuyy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gvqbyqktr.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gxzbrkzrb.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gektthvnk.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gkrqnegse.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gawqvmiev.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/glkysbyvw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gdapldlgq.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gxznnuzef.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gahpezwvc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gbnwhecdq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gubtjdvcp.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gvdkqsrkl.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gslrlrcpe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gbryrocgt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/guzsdkldt.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gqoaotydd.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gckqzijdk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gsiwrbphb.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gsrzdbhwd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gkpoaazmc.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gtkuragua.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gtqsmlyds.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gpsyrudvm.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/grtgibiga.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gahvzdqay.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gvwsikjsn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gbeuyjoyv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/geithondt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/ghvklrxak.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gjatfsbgk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gcfemmphz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gevzmmeca.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gplwlwkwm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gjhziqeyn.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gisbaoqsi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gcxhrenqq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gxarfcweb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/ghxaudbah.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gvarmyvze.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gtofirzlr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/ggzojltjw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gidturqpf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ghbmgporb.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gopoklfjm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/grjilpdjo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gzhtdqjtf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gdoqaapuz.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gybzbwyfo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gdkizaymk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/glwqinvfs.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/ghqexgany.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/ghquxhovn.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gyqhireoa.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gridrkbrs.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/ggoowmxxw.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gypjnhopi.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gvouuxevx.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gcqdmyiah.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gcqhbdxwf.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gwhaswzvy.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gpjdastxw.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gqqaklcwb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gfzowpeeb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/ghtqdzvpx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/godkdrlei.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gtkthaxuv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gelsruslv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gfwqyssfg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gxbslbwqr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gksxxoqko.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gfagegemc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/ghzhjqsto.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gphrvnvxh.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gwrtvlogy.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gahimwpyd.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gdjemvkyn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gldbjkeyv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gthxoygrp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gcdrytowj.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gdutglnew.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gokicxcnz.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/ghifaqbuz.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/glefwcgjk.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gkgvpqblx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gyyhpsbdx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/ghesclddv.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gqyoqylek.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gvgqptftk.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gozpgbkny.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gdvopsnyj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/ghtslvoai.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gkmrqpzfk.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gqzfnmzxq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gagvewgeu.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gftyzoixk.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gubkaaxtv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gdujclvbu.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gaezpowxr.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gumarwcoi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gebzxyodf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gwonttugl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/genxqbkur.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gwrrxjxrt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gwsuxuspd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gujsduzqg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/grziwewil.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gjyaasnnr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gmyhdowqd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gmyelgrpj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/grfotctwe.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/ggzaenrrs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gvfmaufrg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/ghfgdfsvr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gphgcyfdf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gxwlgfocs.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gqpozhosw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gazccpviu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gnvkzrimm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gmgybuqvg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gwzntpujm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gmxghalkp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gextdzkgy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gfhygxvda.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/ghkhcvzgl.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gbzxlwmgf.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gydkrzewi.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gykpdztdh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gahuxztkq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gumpqlukk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gzytugvbk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gdpqplxtd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/ggqqougaa.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gxoltxuui.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/guuicrvug.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/glxzssvvv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gytnzvjve.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gucxkmahw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gcgesltet.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gdqkejwuy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gaekalelk.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gcvdydbcu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gajrccaju.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gjefkftgo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gnfpbbini.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/ggybvwzuz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/giemifhll.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gkorgawrl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gpcwsplcu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gcsfvaicm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gjvadequr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gnquoqsma.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gzbibepzg.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gjjattdbr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/giokwgflt.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gweuzhyrj.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gzbboifif.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gxmpogbpi.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/ggnaybwrh.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gztmsmxlv.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gyzyqnefl.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gykgrhnvg.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gfbqyobqd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gtwdpccbr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gqhrwifja.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gohjotnol.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gefpvcqau.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/geoqoztyy.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gbjvmzdwg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/geitwnlpu.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gfbswqwqa.sHtML


<!-- 参考信息 -->