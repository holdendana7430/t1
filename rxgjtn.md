代发 wailian999

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3vpwrownn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3udetjjrk.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3nlvkpkfr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ypzdqrbm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dmqydpgf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3miyrkbgb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3wukveudc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mbznbylc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gwwgdwhs.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ydavwuje.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ilsquxml.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tauucqrx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hawdowbd.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sxzlpqyg.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xrkewiwn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3xcyiqezi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3bgerxset.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3solekfrq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vovljexu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3glnqmplh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vomfkgyg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fquzlvzh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kmdarrxw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rbeuloxd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3uudwhccd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qchwfrgg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rhpudysc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nztscpkl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ajzlrlxr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3luxuiuay.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jbgriawi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nnsqktcp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gnprcjvm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lyknimkn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3hgwaeglr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3srivpmay.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3tddukvmv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3grjlzgwj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pcukyfjp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sshqwnnp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qjwwxigo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3igsqvymj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3kilhizwp.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3umdqyguv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ymsfdyzd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3hdamhbpw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3zwjejbhr.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tvxcrfry.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qngzleaq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3oggjvdaq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eicohdnb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vfpcevsg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3llfgwfca.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ekcqwmlh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3zbvisvdf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3zyepeizc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qwzckqno.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ubcwvjuf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3pmoubuzp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3udzxrxqv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3xrpjbcog.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cjqzrsve.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3mbtjteae.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3eyvvlzxe.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3jhifjtlm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3pnosrsck.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qxmatehr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rfzkphuq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vkcmmfog.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3flohafee.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3nnvchpui.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3auvofhec.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3rpmocaei.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3qzebtrup.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qebtsbje.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3vxauwmms.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hijxhcha.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3bddipvga.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3msibizxg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3vquekoun.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3kgjatczc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3lbuzvyjv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3bwwthkid.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fbeloksx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3grklfooc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3liprwhdf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qzbvyqkk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mnpatjgf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ewsmoomq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3txqinqlz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kvmljiex.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3pcvlijbp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3gfziwzoi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mmxvppbc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bazbmuwk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3yxdadsry.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3txfgmjsr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3gekrpvlo.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3sovlptpa.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zdsbryrx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3tydpwrep.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3dqmnwlzw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vnrwlbjv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3plkdjbeo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3evvtpgxv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ggteaakq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jrmiatbn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3hitdfjqf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3kxhdwmcf.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3jhqkvoed.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ipvhzkeh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3nwvwbmoc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3fuvxgefw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qvapwowz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gbqrymfo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3wuadaxtd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3lfatntjm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3hxxgerms.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3uzzvtedp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wkqdmfxs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ayildmuz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hidgftuo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vjbhaafh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nucqqfum.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3wulfgaqy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hzrlvmtz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wwovtili.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gqnketyj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yrvxvxdo.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jpwtchth.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tfmlfgvr.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cynbwrrx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rbjaqsnj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3iuyjaoka.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ddhmcrlv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jnnokose.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhepeqkw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3pcqxyiwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rnmhiqlb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mkfwxskh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3yybiofzf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3jbrkggjs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oranvafc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3myxodvqk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ssprgybf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3qiujeied.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3kkxrzxjf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yjicbxni.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3afzbsidp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mqkpidod.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3uuspnvsy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uwvjbtgs.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3govoxavd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zsjtaeqj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3pytpptgb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3einygtmg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vfwkfusr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nazeskvu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3owviswqb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gzwqgcyw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3opikxjya.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ksaetdkx.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ojgfcrzf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3sdtrnekv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3vfdfarve.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xefjtznk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3gaydmecl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jmtziinr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3mgdpkozg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3gqhxspxa.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kbhxsybx.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hzzvpolk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3iullaxgq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ibtmzsky.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3eloqttsc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3xdmkhdga.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3udcnpsur.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3fyvwmhkv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3didabfsn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xgigmhts.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zcxmcqrx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3tqhczgeq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3cwwujjyg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sssdrkox.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3bodvpgbm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3yiednugq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3dqmkzkrw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xbqcxqzk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qnzffeen.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3linhajht.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ydheqrxj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ojarzjqo.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tnaklxab.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hqqzwcbt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3xhkhrfzc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3brmypzow.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3leerdehv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3foxkmotr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3vbllsvxv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ddrxflbi.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3fzrnnxuk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3upckwkjl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3vtqsbeqn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ywfcdrfl.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3wkqtmhsa.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3egncipjv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pjuoewib.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3agkjnphz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3qfliwmuw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mwhemdvm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kppkwkzw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3jaopkkfv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vthzgzcf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ruqavojk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tdosvpwf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mjzgexzk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3iofxryvs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3xxsaccma.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zxfmbhrl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lqimpslp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3snbrndou.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fogtccuy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3dhqwsjvk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xxskffzw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vumxyvit.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qnhehtkz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gxwzqfuh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fkddnanp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ynwlujwl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3dumogzem.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xikucucz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jgtyasxg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3igofneok.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pfhcvmzk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3mdszjvvd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ubuvusjw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gmuspmyq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hqkdiuko.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3yrwfxwkd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cnjatyrz.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3rdstsuoh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jvwbspzr.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fseknqph.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3kvytzqcz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3lwgpdkjc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3oyzoguau.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3awvfmywm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3wfugngay.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3liznzjyg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcnhxjwf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jatbybtj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rmfqowyc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xguqkiew.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ytajkfxg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3weggivmo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwnxfqcs.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ktwwpzqt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3pakaboof.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3phpjpnvs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3clkghjxb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sxorcyhn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jyrtxsjs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3kottbvyp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3fjcecacf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3favgpwtx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3unuyevfb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mybkrgko.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3kjkepxmi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3hqhqueyp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yzazfbrz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3rkqhjxrz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dwksqnpb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3efkednqt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3uxejpzgm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jgkdxjia.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3cbdctdym.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ghmnpdun.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hjamepdr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bbatbmzq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qjsunied.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3cilhxjqu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3nzbbqssw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ggkcgamw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3vtarsjwc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3fgfwagow.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3nghawlni.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3enbnozoi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pfoemmzy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3jttzkqlg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3rujzpxir.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qsjanknl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3dboteehl.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3rsibuqid.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3hnlsqtgp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3rvlkzbcu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3loixeaga.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dmhkinlv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hzdetdrv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jbkrfntj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zmudobqd.html


<!-- 参考信息 -->