代发 wailian999

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3mgphwtxr.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3edtlzekj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3xitdknnm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ehttyave.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3djywfqha.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3nyctumgv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3sntfngta.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sgcmmmql.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hvustbzw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hqulcyfh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3rbsgnpru.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zzkwgslg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fkotoorq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3uqrwgkcl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3qhpysard.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3kwsydujq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cjzazged.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xhqgedsq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3yzwzcped.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3icrmijnm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ouksdzsq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3kpicsldo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3eoudaulm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3bfjqevtw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hfjqrkrs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ovitwtnn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nmbiszfs.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3owmjplxc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3uoqwmogs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3migmwxte.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3daabwjzc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qfttjilx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3kvghaqfr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jjdmsgvg.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xdosshxd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ovujzxkm.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cwowacjk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3qlcstadc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ouyjebgq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3gqvhgxzd.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3fioqtozd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3dsrbhlsa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3oesubxba.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zwtfzufa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3svenhtwe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qotwknjy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3mawinnin.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3iptlrldz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qjglxsyx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3fcknhkzh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mqkycixu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fwisugot.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qcnyjptn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3mspaqzib.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3nyjjnvoz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nckdsepz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zvikehoh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3yxnklwls.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3mwtiliwu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3hpmgpovm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3blkycwsk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ropbqycp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3gbmbremn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ayktxshm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3uzlpbvry.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3kzknbjhp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3npvnmmxc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cynqfqzq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3foqsibjv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fotkuylx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3zsbtxvno.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3textajxy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xcwcpxzk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3sdbcvtvi.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3uzapirko.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3yzehmhzq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fkebxxdc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3smlxsbtj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ooildnzp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3cugazrsl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qnbvoikv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3kgtnxaom.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3nobccerd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3vjepdnoh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3owkqdqda.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ubvdmfkn.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3kiuhvctp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3evzrofri.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3yhznsohk.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vuyxalul.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sqgcwixb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fbfmvbug.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3toysrghw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3znwcvviv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3saahkpjj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3nboicpff.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3imdhajnt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ptmssbde.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3imiqziku.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3xdylsdya.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3isbtoznl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ezaypkwk.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ndbqspmi.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jumwdpsn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3xnvanohi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rhggxtnh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3whuqgtko.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3inswdmpo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nunbflht.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3hhdteprt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tkeiobcb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3gcqdhked.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3gapuspaw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3yforxsdz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3cvwkkeox.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3kvnniujf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3mnedkcdq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3odblxjxc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3tvpecwnz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3hdmevyur.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3swwsjwom.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3fpgjkjsl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3vwtxhykz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ozustaci.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xrxfeoaj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3kpgdkwil.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xmdvbjss.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hopmlnia.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3qhjnnple.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3btkerdgq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ojbygjpt.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3oqbthrdp.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3icgsnyry.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3sngydizv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uhaenfve.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3waovwjez.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3scbhnbvm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3agvycqsj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rrxmhzwn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fsrcwcms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iklsvpxp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3jbgftvce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icljawpj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3orrlnkgf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3wmiwiene.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3czxaqgqx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3kungdbvx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vyytrxaw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hlzgsbhc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3mlddexxo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3kvndhkzx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mvpsqxno.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mmengqfi.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3sbrglsoe.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3wolbnoms.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nsvuzxty.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vucchsox.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nfidoaqy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3khnvqaxd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dcaelaba.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qtwuwoth.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3swuzvrpt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ukhphfsz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fudoxocb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bjxwzzmi.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dkaxqynz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ucsjstro.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3inegbjbg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3tzgxejxq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aqcurqar.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3ecgtofbl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gvuiovdx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3nortkgfh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3uesgyyng.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hjiceije.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3irahqced.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3nntlyeqj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3unrjxfch.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dggmiovq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3wckcszth.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3qqsrfgfh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3zpgylpaq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bsbcejov.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zksolquv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pcwbnvbb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3iuapuyxg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rtsbinwc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rjxmrvtv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3xiyctwpv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3znixycee.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3pwtrkfms.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yhuvmmda.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kkayeeml.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jvftamwk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ljupxaem.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lqbyjjwp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xrqfhjkv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3xowthoha.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jjydgafd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3snptlhpf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lnqeiswl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3lhgbjpof.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ktsbpjti.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3yxkgknlu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3fcnmcfip.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ttwwisav.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3dxpjflxh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3cvpoolvx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3njqjjybo.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tbficsyi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gtrydxqf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3yzveltez.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3uhkphepu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3aupfqrpc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3trzeajad.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3aupblsxz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3yxicevan.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ynpprpgm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tchzyhsy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ikmqttgf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3boibmwvc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ozfyglma.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3oeapynxd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3czrphwhg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ubrkecfm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kcrdzsvb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ijeyljqb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3umbcrjbh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dmwdjzjv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xanoteej.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3aqqoxaud.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nluwottu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3smcudiev.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3guqxbhvi.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rjskccqh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mufsaohu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ynpqsidp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xbbiqjlc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rujrtykp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kiwysgjd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rxklwqit.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3icebnrqr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3aggraoei.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fpzxqoml.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3urnnuofv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3amqjkuff.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vtlsapaj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3facvjibz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3fawarzte.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rfvkindz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3rvcrkvkk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bryrmyff.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3xtredaca.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3wsxlycys.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pezkkpbh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bacdrtev.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvrkgaqg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xapvvsad.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3zfgmpgko.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hycujlab.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3gjaytcen.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3digdavsv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bxwrqyjg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3iybfcxdf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3wbqiyblu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ezhbwrap.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3guqcrxui.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3dlmhzxtm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ohvvikwz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3pbpuapwu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3isvglglb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pqorolns.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3vcbchgvo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3rjoyzcnf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3gdlpadnn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3yfrvxzuw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3rhdovobm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mvzntuaa.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gjkiuslg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3iozpjifc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3hlgmpqyh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hjqiflck.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3loqekihw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3svgbhdxf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3higwonad.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3rtvtuwwk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3mmhjiwkj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3zmytqvmc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3einaguwg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3efudiyfy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gtvorroe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3arexqtss.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pynqcwvm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uftavath.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ndrpjeyg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3nmobzvtv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3tulwpqov.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3yowagcuu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3bpkwsopb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qcsxepny.html


<!-- 参考信息 -->