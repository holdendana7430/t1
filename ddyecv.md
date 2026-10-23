代发 wailian999

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3dkywdhus.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3lhsywhum.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ajmerkmn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3wimwmhly.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zxysrsmd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3xzhkbobx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kzfsohlf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3gxcqbxzt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3qpkabrfo.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3iownvhir.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vtlnjhat.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jcyqybks.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3buzwswtg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zoiukafr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3sgxujijl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vnlddrtr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3idmfbiiv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3xttnrypl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3svkeudvt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pydonnjm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jeuucgxo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3livwwthf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hyxctlhn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ebxfccfc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3thsuioam.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3mdigwzyu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xmtbecio.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3vkjugbim.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yvujphkw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3yhaesitd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ensbezrb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lorgzazz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gaprrmry.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3weghxelk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ptfvtgby.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oaxypdzy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3dmabxugy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3cbripvhk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3gkditxdv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3alqleyom.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dibyyjoa.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3xppknyxg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3rdrbenko.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3oqvtiajr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bebptawh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ygmkwecz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yvmuroef.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jleehqex.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kczoqogy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xfijulcs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ghukciwh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3gsokzxon.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3gsjendiz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3mlajbsto.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ymcwkxeq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mqysseaa.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3upouzwpn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3gcazstbc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pmxogqrv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ocslfpae.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tatkabak.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hwkrissv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3cwtgrkgj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3gfewntqt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3dgfbkxig.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3pdlyjrkn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3glnyhuzq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3vjgvwrcs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3uibjvixi.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3nednryiz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3fpqjfscy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hpxykiwu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3utfmhpml.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3vjgqhhsa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dsoknkda.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3donozeog.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3cigfrmiq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3yqiehgwv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3yrjqypzu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3gjapaazd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3rlvvdwxm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xkwrsgqb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cjdlmgnl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3xracvxzh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3syeqfngo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3nhgsjbec.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3qwleklud.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3wbtixama.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3qblatlsl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3noucnefe.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3vzdciywh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qpzawbcb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hkwdbkvy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yhpyslyn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sjtmjnyp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jjlozhzf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qqijgztg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rjbzydfz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ajlbaktx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3tzqolumm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3edozfphp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3kmgeghky.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xkruvjch.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3spxhwvfu.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ynyzrdra.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3jkrjtnuq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3zqeqbkzg.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3plwfnjgd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3jcpzlkuf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3uavdnhxh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ykmbqzfa.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3snsdxxvj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3stmkexmu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3jalxxhld.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3sucjymeq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ubuefzzn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vvrmvtwj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3rxbptbzj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qzxmobht.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ozrlvbxu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3evbjciup.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dapkynlj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3huzbyrjj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3vovdqgqy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3nomibknz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ykpsuaxv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3wanzeypy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ouudduwc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ihpjiodk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3honyckxl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3cjbnuurg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3qtefcmxs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3didqxwno.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3yqcyzbpg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qkfautrq.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3szeuxqsi.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yonaldqy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qxaxsioi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3nnxyhbgb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mnjnqvpk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pbujxthb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3jnrhyujr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rhzcenmd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3cbnjifrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sccgxkyw.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3pcdgzioa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ykqqwbhg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lbxubgpa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3mktfhltp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3gxrdocdv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sdqaqmwo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lsmbzrye.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3feisvynu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tgdzydea.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xtimfeey.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zjcsssbu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3hfakuych.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xktrinfq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3hhdvvjhb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3robwnbhz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hoxqsbln.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tdyfaffj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ltgqggrj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tlhqmhbo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3cgqyonkg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dswfypcu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ysplehoq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iagwotnh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dbeqjyss.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nmutitxc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wyqxuaip.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ebhpysku.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3tcnuzazd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eafmoznk.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3iazhspdr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zjoyvuls.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3jomhspdn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3aqmekokl.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3namoccgz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gsysfnvs.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3gfxhyjdz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3icmnrbtn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hwihswaj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3nvdcafrf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3lzqvuenk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3nyeiydxj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pfycovdf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ynunbugj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yludscvw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3gzmqacbi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3teydzbkt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oabaanie.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3djplddus.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fkbyqliv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3mjwjqpfu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wpqotwfn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3evqfwkmf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oacphzgt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ryrdkjeb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mwiwgias.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lemeewef.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3nykseztt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3oosevain.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tajdbdvg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3yzhszyzj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3oouodjqh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3omqdayzb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ivybexcl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ctjdhurs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3dcashygs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3gsfrxkyv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3rnkkngdr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qvfunici.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xnszyryi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rfgiflss.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3bptyjvcc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3csyjzrtv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wtbocjoc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xpjlqtou.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3upuogudg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3vihpskys.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3egpnuwks.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lwwefrfh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3nctiwloq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vvcuuryy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3gxgebmhc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3rbojocql.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kbrlaouo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3pahjfozp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rvwjctyp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3pqgioblu.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jaqwujaj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wwoxirfr.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wdadrcez.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ulhddxqo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tgwxqbbw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3eegafjns.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ggvfhibb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kixojgwg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ledgiiwt.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mjbcbiji.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uqduzumv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3hzbimkvs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dfpbykqm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tcguzujy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3acgaetcw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gmpxchwz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mkdguxst.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3eqyggvwb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vqjtyfum.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xrkjtgmd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3iuxfyecw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3uxqifwee.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3yyncdwrj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3zgbxcvgx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gyvkqwwa.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3abmwhnas.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3nvnevune.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ghcprnwv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3olkhqhke.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dxasoszv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3vylfgpvx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3twsfirgt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mcigbwcd.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3lsiiywcj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3tqhlzbcc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jjkvsabz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3chvelidl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3xpqjekmc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3urvpnfco.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3anhjkwpu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3kfamxlnv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tyxeklil.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3pwqfpfkx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zhvtmisc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oavgdwkl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3oyrphbai.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3zefdzhte.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3hdhibapn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gozpffdy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3srsfjufk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3dswvnhzh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3uwefrfnz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3jaliowwz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3tefozmsw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rjqosuui.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3frylammu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3yzgfjlhk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3nhntpppk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3burjdaqc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3tcouggtw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wythayfj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dfnfeqbe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3lysjhmhs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3urokeczd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvngqecn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3fysrhtzw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3msxvomcv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fdroprgg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3cpouwamg.html


<!-- 参考信息 -->