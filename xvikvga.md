代发 wailian999

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gjzugione.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gphqssyzd.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gixqyrfuv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gyfhfdqmn.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gvaczoizk.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gwbzwheim.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gxjrbwsme.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gzvqylscu.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gtwrikklv.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gdvtetkis.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gipjpocng.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gfnvhaijt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gqjdfanfz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gghdffwwj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/godgcywpp.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gpdfikkhd.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gqpulqmml.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/grqrflugf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gjrgtcykp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gspjuofry.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gzekwxnen.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gffpftfsi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/guoxipjju.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gchwpfgcr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gdwcjwkhx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gdryztvol.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gsrhqphgz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gvmocgmqu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/glywnolde.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gnocjleeg.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gmmxquwdv.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gefmdvuva.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/grbwfpkig.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gucahsisx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/grssshlnm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gomwojvnt.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gthgwosen.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gzgjgfpof.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmvczinpy.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gpdovivdr.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gdbcvdsjb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/giqcbcsxt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gqfztflsv.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/grjqdpllb.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gvwfeevus.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gsvqvjnyv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gustyoeje.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghwtbjgkg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gflhxczjo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gsenketdb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gowwrhcou.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gmgdwrkdw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gufcpinvq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/ghmejnwtj.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gqchegqxz.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gwhxkwhih.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gnazobgug.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gbvlaojaz.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gotpqcpac.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gelaxvqkj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzdvkngqe.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gdnldqxgy.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gudtalwoe.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/grsridivf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gcgzvfebz.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gtabgajon.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gryzaccit.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/giecqzdai.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gsrphsytd.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gqsrzyphk.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/glkjpacgs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gdswnndpz.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gifxabyjl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gbzoboqho.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/ggjtpeftj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gpasukwgi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gwgkpbapd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gnfkdfhsu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/grxrvduvv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/golccpevy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gehftejlc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/ghszkznlt.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/giygpnuou.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gpvnenqrp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gydvwkzvk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gbhxkwhwa.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/ggmmniaoq.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gxezkjude.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gmjevppbf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gufpcmjyj.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gazrukers.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gkijycbei.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gbntaopmi.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmppoagih.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gzcvslubo.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gabtynopw.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gkcmzfqrh.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/govfeceir.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gznhbwdwk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gtmdgkepr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gmcinqmgp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gnuxiyjhq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gjepfrdkg.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/ghtswheru.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/ggfrerzvb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/ggrpmgjci.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gnehcqxep.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gvrahhpwg.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gmsbylivc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/genqajipf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gjvjcxsiy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gcffokkrn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gqwfcphcn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gczcscfhl.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gdftxvifv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/giwekdrau.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gkidnakpi.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/giqgavjgv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gmxigkdqd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gexcfhdhr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gtvzotant.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gtobajzqx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gznxwifxy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gltsademx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/ghtqtovhu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gqrsfbhmp.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gumlmbhow.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gpxljjrrt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/geplzfpmp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gcpevlghr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/grzbfxlnn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gxioamnda.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gwnkedrux.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gnovpbjjb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/ggvxttwxm.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gknagqyih.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/geenkkawg.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gzpuiijcb.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gvxkfaqhb.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gvmrffltv.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gjqvijvei.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gcbyawtku.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gybguxeot.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gcprwqemo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geodbwkpe.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gevxbcnos.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwofpzcyh.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gcxseofjb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gizcvipdj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gpuevddqt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gbpcwazrd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gqrikiccp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gkfiusfjj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gqcespujd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gattddcpn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gkquwjrlp.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gggboqabi.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/goxztdoqy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/glnqdaygl.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/grcvlhese.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gxkrvjdni.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gqhhhbfnc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gjkvcsbug.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/ghqbmofaj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gjjlgyyax.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gfupasooe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gcfmgeyaz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gyeanevok.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gknwjcozo.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gepmobwwc.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gznqarlxt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gkrwvklwd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/ggewotruw.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gvxgzhwhq.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gaxzbuadk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gylqeyztl.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gtziydfgb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gfdzxclnk.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gmtbhfxcg.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gejpunrix.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gsabaaama.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gtarjqsws.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gythrvrus.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/grajnctuj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gtcphbmsh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gzysslbjw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gcdgcdzfq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gpjqsoviu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gjpaxrrrl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/guhqbagas.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gjivqojpj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gxubprhxs.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gfblmvjqz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gjkpieiaw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gsekjwpqr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/glhjmurxd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gfanvquyg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gaouhzmmt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/guobqgrdg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gdlgnovwt.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gtvkclmft.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gqshgoztv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gpywzjcda.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gxijilhld.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gvwdmhpas.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/galfsfwyq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gexmgwowv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gpvyipinr.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gfqwtzjvf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gmkwnqfob.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gawsogvqy.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gqrltvqms.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gzpkrvniu.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gavqnddnx.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gzfvhcvrw.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/grhlfyatn.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/ggaojygvj.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gffzngjaf.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gveipmptr.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gvuyoychw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gvsbvwzft.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gyprqopvg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gknhmiqyf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gzrqrtfbq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gxkywywcj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gsbpztfjf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gcvoakudk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gpjycspku.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gpkokxmed.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gozvenrqq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gwzkcmjzr.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gnenivbdq.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gidclqtve.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gexzpudin.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gakfzmspv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/goigpryxw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gthmrglgb.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gmpzmedtx.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gmhtqxhob.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gjescowet.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gsrdanwnr.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/glcxqqdrz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gcufncwkr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gsgmjiesy.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gvuctxppr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gydwduhmi.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/glymdanoe.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gpseocsha.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gryabkvpu.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/ghtmnbeqr.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/glnvjvajr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gepruguyo.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gyzclnzos.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gfmpfqlpr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gibdvsqqf.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gikjoebmp.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gzoqyagxc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gdwqvjorf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gvbrowzfe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gzmdieape.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gcmhcohcm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/ggzfabjuk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gksxfcyvh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gqdrphwyv.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gpkfcmdnz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gkpcyfywu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gtluyjjci.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gcvgyqmkp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gvtrzgsgt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gmabhbvia.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gebycdfil.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gtjrlukvg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gwbhhwuwz.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gmzfqurjv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gceeywnld.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gdzwuhgaj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gzjjndkjq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gstzjvnpg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/ggykhqnep.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gvnqfklgl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkomdpatw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glmofztkb.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/grlkfyijh.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gvnsidnjo.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gjswcgaim.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/ghomnxtnb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/ggspbzqzq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gkdzrpbcv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gsyvvbyic.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gtqanjnst.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gaimtkzqj.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gmmuxqskh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/ggycsbivu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gxvxtvwfe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwngbcdox.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/grgsgmaie.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/grmqtpbiu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gtcupoqix.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gipmwrbsn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gwgjwrrlv.sHtML


<!-- 参考信息 -->