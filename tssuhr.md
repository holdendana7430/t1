代发 wailian999

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zqiwuiug.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3cscgobcd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3wjsopozj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3wgskuxsf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gefphtua.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3jgxsmcwp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3oczlcepj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vyfbkcpf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ktfovynd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ldfnqncl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3bahgrkez.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hunxuqpa.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ygivyuaw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3hdhjdfxj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ibqlejxh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3cdyczleh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uasrufif.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hinbdwsj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fprsctep.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3bgalwxxp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3uiijjwvn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3uwdjenjz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zcigvfdq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3iyunvnql.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3htgfxzac.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tsstqnmm.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gipplyhm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3eehzgztg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yggqhnum.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jbajhwxm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tkfdhhky.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3aiifxwdl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yiusnkab.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3kakelkhs.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3lhspwhhs.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hzstjtoc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vscrnpdh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3lwawzdrj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3rzalybca.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3flcremfl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dpwlfbef.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3lnckqytw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3llymfwhb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gkrfdsbt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mmmpnddh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3shiuhfvj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3kdtcokbu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3lcxicsiu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3lmmgishe.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3vozaulxm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qfqmuzzf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3uoibjlty.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3mxxmhdwz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3vytaxtsr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cplyabiz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3okdizkak.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mobxriek.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3afbtvsfp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3twnezudh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3cfvxduvy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3cgcrvbut.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3kumvydzz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3xokrhtxo.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3qvwqxvwa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nnrvitcn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3dimfrttn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ykavksjn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cvgevmqq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3wwbymjvx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gssxydlj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ljbjysof.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3lsqohuab.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kthahjzb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3dxapfomz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3bndhinwg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3nhgkpmow.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ckhcnpfi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xhppfnjv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ovnbushq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bhnaebbl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gztlentr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3onnolcqx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3iudqhupm.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3utevgrbp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3kmibqkdt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3tyqisijz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3clbgignb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ncnmtpqr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3hyqtrngv.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mmkfityc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vatchohg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zvigigrt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3evfplcar.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bwyxavuz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wqlaeopv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3xeuklgvz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yutuiyrw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3wzosvojg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3etmcjnbs.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3puxgfrsy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3igxowqko.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ihmfzvlz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ibvtipta.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3znhtsswo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vcosbwcs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ofgsyeke.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oaestmpc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ooqoxqtd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3knwovakm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3zopyketm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3oksplrmq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3oqnxseow.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3fxyxuimp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3fgjfxfdy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3cnnzcccd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cfakkahv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3msuqxkfb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jlhxzxps.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gckeanyh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3yfdcpaaa.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3puzarkdd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3tradyihj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3bedyuvwz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rniixodv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qgecnwhq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vykzqpxd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3fyobuyag.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bbdlyukb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3eycgcylc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pgddniun.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3apibntfo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zraxihqz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zgdcemwd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rwnkoapf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vifohqdk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cruxpkmg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pctuegxr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3jgrryswn.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rwsjisuu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3abfedtsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3weqolquy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3tovgufli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbwvcmtu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eadshoaw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3zbhtkvgu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xpgviunb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wxukkcpo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3hermjwlz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3fzvzqepx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3bcontwxj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3gwzskddr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ihwltdsq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gfkhcjgy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3huejdtgx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bgsqkjpp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gwcdssho.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yuwcgsqd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3polenqlr.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3extymzta.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ydblodcr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3fplvvjmg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ivonyezi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3jvmwzotk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vpxalfrk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cbawhwiz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tnctddwv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yvnhhbbf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nxcbswmm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3wqjdbrkc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qkiuhdmd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3mbjcqgyr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3txnytulk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3crotzupw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3mskbwxxl.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nwujyhkf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3airrpyjg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ijiargcl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zxsbmwsv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dabnwltd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3squvsftl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3aqttjgts.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3tugmrswt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ebauacyi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jppoawgu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hdikklic.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3nhwmmxwi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ovvhjriu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3eifkphtp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3gkujaeha.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zkvmmfnm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ixtixgkj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xkqocfhh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3frhfyvqa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3glpsrxcl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pptliglm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rfvuuaiw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kvmyorzp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3lazqvtuu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3faesmrux.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vncgolit.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3zwrjvrdj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xwisjrnt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3qfaepztx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3souynsct.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3dazkbyof.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3gkbkenlb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3yvogwcqf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3mwxcqxms.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3wvqckymu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kflloync.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rckhbbub.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pmdjalcq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3wzyznagb.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wwrizvdq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gcmdrrpz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3dxrzytix.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xbulkyxe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3czlymgjr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aajzvodh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3oviczauw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3togpkczo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3jfziilpl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3omkvctvo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pbjskakf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3crfjfpei.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3agovctyf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3yqrtlvxi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dzhbkhuy.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zcqfplrr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fcpxipat.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mczwezjt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3iggknpyx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ljprsxtx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nuihybio.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jpndrjhw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3lhusuauc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rhfjnnls.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lrwxxvlu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3azovuhys.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3gwcjtijp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nkxsxswy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3psgczrtd.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mzgmsakv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wvjommuw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3udnredht.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ndckbblk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dyosafvi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3lhpmwmea.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3umlvgpqr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hjfnhyih.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3uorytpqi.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3nvruwmyg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ywkpbpmr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxnuvjcn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3osrwdgue.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmezyglj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ahxsfhai.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3xzdglpvl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3pwahskkj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mejlgezx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ipxcsfbi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3rrtkbrhm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ajzuxejx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3wnggedst.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jnmaizth.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yavxogzv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3cvmfnmrh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3lmxvbaln.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cjxqiseg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ppfjnqpj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wsoiqvoy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ojzczkir.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3pyugniog.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nbvlzrbc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3covmnurm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ctpyvncl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tlxecbjp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tiuhmjfw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pssogbad.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3xrohvqjo.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3egszmlnz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3tnarzvgv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tstmmmel.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ugttihbm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3buyzpauk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zqpcfejz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3hlflrbsr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3cncscrvd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3iwezdgtf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3aghssukr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lhsikcnt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3frduxhpo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3mpohkcvs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3vfoqtetn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3oqgvmhej.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3renksucx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ebpbdwze.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3tnedyqsy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3agvelfkr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tdfznmlb.html


<!-- 参考信息 -->