代发 wailian999

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3asxxuzdh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3kcesbxpl.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3glpxxlgb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3bcvlhhle.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wtncmebb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3udwvebuu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3udqnnyhh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tqvdxdax.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qpzkanaf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3cfkoarcl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3byiyynyc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pgploxpj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hhdluexr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3aoptzalk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xjgjwtws.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rxbrdvzd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3valpplpd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3drdttrxq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3lzywwukh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3irdxoptb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3eatmifab.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lnerrlyc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jbpoerzk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3vrbadfop.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3fjvlepmk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3btixjdcr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lorjxuvz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3esnsscpo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xgijopam.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hupxdatm.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nucgaygf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vjhbisiw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3wqtibjuk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fmknkzkc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dbijazle.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3edgefxxv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3rwfvbabq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3atoxrbbu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3vpmofawe.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nwdeftzi.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gjtqcmyq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ycuiprhh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3estbsrse.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3lqprdwhj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3jcgdodyj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3kqepsbbn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qswsccmo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jpbfqpht.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bfpuvmsx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mxhffbtw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3jivekups.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3jdgqoyka.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3udplgnfs.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3vqqhlcra.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3aowdyiyw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kksgjtzd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3fyjpbqto.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pwvlwfxc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kkacdaqx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3actxloog.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lvwthonp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3gntspusv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ugloywqg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3xpvthnda.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ngecbans.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3nsxszviz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3swrgbvro.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3hlyyexul.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3bbloijhx.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3gvcpantb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3mahczlya.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3olkrkdio.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3fjhpnqch.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3dsisblyv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3usmwjdvz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3gxcorage.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3yiswnpce.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3boaqenqg.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3htjfejay.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3lpidvare.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3otwogesc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3wubzfddf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xmylcmwb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3emdmjjje.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3effmzlpk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3lvbufwxy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3wjzseoqu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3qqrbhiyk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ynjstjhi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ebsqprwb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3txmowkzk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3szicecpp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3kjyyxvnr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kpdtfksg.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mabispkd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sqztndrd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rzeyqwwy.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fmhahlmq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cjbeiyoy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3tmgxakop.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3easbdiqk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3jjlvriyo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3fskuqcok.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3uqjssnwd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fjwmezrk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zbukcbjf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3nfpeygfo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fkyetwrv.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dhcumezb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3hehcarjz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sxsbcupp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kwrzkhut.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ajkayxhh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3xioghkso.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wyvqunts.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3xayjnpjs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3lkqcbbeh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ysaayqzi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3szrlmfde.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xkecinjj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vykwgner.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gvqdhjiz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3eqsmvkxl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ygrcvlio.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3psqzcupn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3klsxrild.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3dcddelmq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3roahngvt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3yrclbxxg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3svchrurx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3zzpztslm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3apptczjw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3wyucruoq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nigtofcw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ljvxjzrj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3mliejpak.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3heokohlp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kgdvxppo.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3chlckmnh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3cfgmrhfe.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dsyeluky.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zjldvfnl.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wijstvew.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zhdieque.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ykywqeyb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3qtlulozq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ohzjjlag.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zqobvkym.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3rfautaiv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ynguqifo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vgygxzek.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ubwbbcuz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vghuhlzz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wjzbxbew.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xdlpsscn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3krzdxbty.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3bteukohk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vrtyieiq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3nshxcmeq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vodubbxs.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yjzrmaor.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vafdnwpa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ezgqdraa.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xoigszeg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3aioqwbkh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hhuxppnz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3kxalikrh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vwtkwvcr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ccfkvfvi.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kswrmblo.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rajpsgdl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3sturfnyp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3fjwctrck.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3srqxsmbg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3nzjtsgyt.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3epeqengb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3lqjlnojw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3siwgtafj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dauskukv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mbsoleas.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3gdnkgroo.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3agbmgeay.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xdizizzf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3axsfrkgw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3pwioutol.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3wdfwkrga.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kdyykysf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3mrrajxrp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3eimdswui.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3zzktqwmk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ondmgqml.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yysegvww.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3shppdets.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3smanlwwg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3tvtfvdbm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3itfybcuc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ehlezoft.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zylpsqyn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3prnkvzmn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ohlamqxl.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mhgdiriz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ovzzwmcf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ccensvxj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kojlencz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3pmhsmusf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fpzqrfnt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3cujgtnjm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wnclppfq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ccgupeze.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3mxpixftp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3bbyzwxue.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3pdqdehrn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ifmcbicf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hekgxorq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gymtrkia.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gcakpahy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3blgfrjrz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hxabjfrb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yvstdvhh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3nwyvzidi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ssbmdgjz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wxsqnmwv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3aztmtqex.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ggmlsouv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yqloumqf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3fsrabplz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ywviyxmi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3albvblpe.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3nfewkjzr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ofxwjoua.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ddlbavcm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ibklnkuh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ezudovsb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zakpelpu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yjopgvfy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sibjsghr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ttakievx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kbxiisgq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3eopfjiwo.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zdwuxpez.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gdmoqfuw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jdfxrpxy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bsacawrg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3tpmahfnd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ljvkvqme.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qfckvvci.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3wdbekoec.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3yffyontu.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3mcfbnood.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3affoorhy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qdoygxot.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3zeadwrmb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3qpmsggdf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3cxvmjnif.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3oraqdmpi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tnzjzblq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gwirgdss.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3tvmkbjwo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pkzbasil.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rojgcavb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xoysflzx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3aktgvazp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3hnfuyqyj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwwfudxl.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3pxwomkzy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ztgxgjkb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nyspdxur.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3libpvydm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3chdltxnk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xialmckp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3jfpbkhup.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3iifogxfh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wldwigrs.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3cjjbfknl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mvprthzx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3vasrfdzv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yisobfhc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wznwvvqn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3nvdcbcme.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dkvkfmth.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ueebftwn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fvzpazyn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3cfmpwwzh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ffdudzte.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ubgtevzp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3btanalmz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fcbxdnsn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rvaupdkw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3sikiisoq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3dxnqagdy.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3bnjqgdjy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3mbzbeyjk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ejtbjkgr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3exwdxntv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lnehodwt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3kkuapsqv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dpxiwxhk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3zbqepuan.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3phtahvxl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3rdggmnrx.html


<!-- 参考信息 -->