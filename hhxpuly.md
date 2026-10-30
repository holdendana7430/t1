代发 wailian999

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gqkalaoze.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/ggckxgsap.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gixccxipc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gjdbxegbq.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gvrrosjks.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gtjkutggy.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gybbilffv.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/glfnmmdsg.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gptugobcq.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gkoicgsbn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gotyjxhkp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gkfmlabrh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/ggwsirnco.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gxtnhemof.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gogphvddo.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gbthguefg.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gtikzcbpw.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gumyvziuz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gukyercbz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gxiplwkle.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gecikeqqz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gybxkirch.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gmramlkfn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gojmzwlim.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gcohugnbs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/glfmzlspg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gdmdzhcqj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gqqqhwpmm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gtgnozenl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gdajmxywk.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gecyxafqp.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/guwpulzzs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gshohejwm.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gzrpkvwpg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gvfzisyjj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gaxjwcxdk.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gvurcturo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gkomawlyl.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gnujiyibr.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gscarvcmj.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gqiyzvqcw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gwylditou.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gwwoosboo.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gnzvnqnrb.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gksktsjgj.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gvkunswdm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gzfyhkdov.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gogwtaiot.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gtpvjgcom.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gkxkudbpz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gcknpxdql.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/grqxzguvn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gluiihflx.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/ghjocmdck.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gmyllvmmy.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/grxcvfrts.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gxconbeoo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gmjdtmcfy.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/grcgxpiia.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gahmtccrs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/ggpmjmurq.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gfvpigjcm.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/ggbgdsvha.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gdgnuqvke.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gnuremqzu.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gqcufkhoh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gfobbpcqs.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/glqrdlfer.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gmxuwqtds.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/ghzauyqtz.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gpowfhjgl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gfzydjaio.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/getoysled.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gasvyiped.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gdhdoackm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gnncvsuqy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gbcpxedex.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gaxywhupw.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gfgjuxynf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gzkxgaeat.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gbejjzemn.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gxvppgubz.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvuuwicjd.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gxfftmiqh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gswmftiuy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gbguubgvx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gvoxmoojt.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/grwxsawja.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gtpwerboi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gdquospyq.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gidzmloox.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gsambwugd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gkswqwqnz.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/grxcbbqbe.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gyqooljpp.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gljofhsfs.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gvdxltgxt.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gslbaboeo.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gacpmkijj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gokatxhwa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gdfftsutr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gxjzrljzm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grmpteztw.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/grcvnbqyv.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gziqfxlgz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/grxpgrtox.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gdhcilzve.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gyxruxgwp.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gizhjjzcj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gwsouxljd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gdthgckny.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/ghhmhavjx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gykygtipy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gqrjohabp.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gkmpaqzzj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gywpnprpa.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gzowdatse.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gcoedjdor.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gipgxrvru.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gceqgtfxj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/geirronww.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gdncpkvvb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gionmvjbf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gdhnxyfwz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gpimzyrja.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gtmyhcgbr.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gptmwrsab.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gltnoswby.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gepfncoex.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gdtdtcazo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/geczaqadv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwunyohgo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gksdohpah.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gmohvcngt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gwuepkosx.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gfswthtcf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gaeiujrny.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gavayswzy.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/grmcbuiqn.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gmecfyhcs.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gatjzkgdi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gslevdiuq.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gczupxukj.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gurprcfak.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtlyrceqk.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/guudsucxy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gicfgckci.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gkjzaruyb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gcpzwwdmn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gacfcwgov.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gkuwmbptl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gkodjrtpv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gvltdfwyf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gqteohufi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gwfoyfwpu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gnhzxhynp.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gmojjmopg.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gcgeskata.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gvweccyme.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gzrbyvgau.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/grhtadppq.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gyrhqpjzg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gaxnozcio.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gvfzfodzv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gtprvieew.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/guzdypogb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gahqkksqs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gmlhqstqw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gfdfrcgyo.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gwwgicypn.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gbektfkzq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gmdanzaco.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gqnguqhcx.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gbloroldr.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gjjcgfmbr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gqfubtsuu.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/grekbpsrg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gchmybnid.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gqxevbbsz.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gxkegjjti.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gushrekvj.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gzxautrsb.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gfgvwtwyp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gnitqjsph.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gfxkhdrsq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gcvhnowqn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/geirpundv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gztkqvwev.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gmrqsuhpk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gkgzcyiqq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/giogbybgo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gusacndly.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gnocuwblz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gqrogrvzh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gowoawebo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/giavzihix.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gyvwrfomp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gbckvydha.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gguiaqqrn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ggonvtmjp.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ginvpndrh.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gqxypuvrr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gloyrrhyx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gjjfrrsby.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gaarfhiov.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gpcpfthig.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gcgcqwgxn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gwchiwpbz.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gtvheytwx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gjzdifgbk.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gcikqjrxk.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/ggsnhuyoa.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gepxnyzfj.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gjnzvorrw.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/ghsfchwnz.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gcxfgqnsm.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gcrtyxdhd.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gqjcoqvwf.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gystlqsyy.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gkvniehog.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/goofujhnx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gtvfyzwmg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/grvtovbxj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gzuretzhj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gkafpnbkr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gwckrydzm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gqwdfmtgg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gzdfvrquh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gptfujhga.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gipvyjgkp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gayqcgwqo.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/ggizzckxh.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gtvvoeauy.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/grizlbcjc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gbaobgjmm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gfdcyesgv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gwzcbjkbc.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/ghpvrznhr.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gworozkml.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gtjvxlpsx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gzjdhqkvp.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/grewidsbz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gxkmvogvw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gcnnidzvn.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gzjkmalal.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gqsimeunp.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/grafszbud.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gpsxsypux.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gqocdaxyn.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/ghikxayen.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gddarwuba.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gnmhofkwz.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gvfepochr.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gncqsdqac.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gkijmrbyi.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/guwnlxlbp.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gjxpmtuaf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gjmirxxjz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/guxuylmkg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gybfuofvf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gonsgkjmv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/grtqmecvu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gycsbdoxx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gjcidumwa.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gcjdwvadr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gizbwblpc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gosjgjnpv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gbafozpmx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gheqrtcyb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gjvskvvmp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/glkwwoafr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gbgkgeygd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gfmyngqlm.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gmswhwmgx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gmnghgzfp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gpkdewfnc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gcnwwcdqp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gpbxninqk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gefahboxk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpbnlrggl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gfmtrhaib.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcpjorcod.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gblxhcmpi.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gfgievvki.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gwxdywcwd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/ggzamidwx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gnxomdawr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gmutplhpb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gzzkinlgv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gynsgvzyv.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gnerbypth.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gxgthhyfb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gqaxshxoq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/ggrwhpgqc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gofycfpbo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gshxreynn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gsaltdpid.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gnzichnrp.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gommucvez.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gkzluaosx.sHtML


<!-- 参考信息 -->