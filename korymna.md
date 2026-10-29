代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gqepnhcqf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gehebyciq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gmdyeputa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/ggbwvdvoy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gikxchvbt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gnlrbxloi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gfkdvwdcr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gsuivrver.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gnpugqung.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/ggvibtnoc.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gbavlxbby.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/givtxdwop.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gptxmjqiz.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/ggsgoxhpv.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gixxvoosu.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gqaxnczeh.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gvuoiwqzj.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gfejwwifz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/guewwrvui.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/gbwvjtqso.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gocrwfwdi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/grrsqaqry.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gzrfplhun.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gqhesyxns.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gvmdpvziw.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gtmvqgjew.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/guizqmvrk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/grvdpkyyu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gkoxcvopy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gtddonftv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/ggdlehhyc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gurlbrhhe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gnhwobpor.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gykzvbiwt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gkfbmcuid.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gnkbhrdgr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gmngilmvh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gghyhzylo.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gtnqpiczs.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gyqnonylm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gexigbrwa.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gxyfsbive.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gbuaoejqo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/glzwgoqmt.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gelszgtso.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/glczfepra.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gqmlcvgko.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/giaiixczk.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gemsbnyxn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gdkmgafpq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gdmmnxday.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/ggjmaqsny.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gngxzzfcj.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gmzzhxoqa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gxuljtdty.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghdncmclv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gvntvdobn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/geipqzvrh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gbpgfkxac.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gzntppgui.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gmxljpmdk.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gpjbmdaqi.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gbgasfqxp.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gjfupyzfi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/glgxubehe.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/glwircnby.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/giawoqmvh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/glmikdlxf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gwdocibkw.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gukjkefcj.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/glpzcakfr.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/guqmwrwmi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gbuziwnqr.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/goimreawy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gtseoklhn.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gppfnyinj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqufzmwjp.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gmovtmrom.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gjdmcpmye.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gluefqfvy.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gakyoibhw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gwuezuxnc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/goqafmoox.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gtwahsgrx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/ghjuseyzo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gkgidesql.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gpbqofczi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gtxqpfjrf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gavvwuusi.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gnojhoahs.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gmbcocvup.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gyaxlfjis.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/garrlgpfj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gmbrfesch.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gxivipdsk.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gaqlzeltf.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gpvpgmjnk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/ghlgvbimt.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/govdthjdr.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gufwffsqn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gfrorvkko.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gxjfpproo.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gqlljtoyd.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gnmrtnojn.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gyfuaqpxo.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gyeinzzxc.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gqtmzydon.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gnuqllbrs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gjhlmzuab.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gkfkbyxru.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghwewtcxe.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gpcflasdv.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gkxudjilk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gkkzdbxjj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gihhtxdun.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gvtzlpgqv.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gwtdrdorb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gbffsoumo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/grecxufcs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gormeyzku.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gkobnkixz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/geomfbixr.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gbfcbskbz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gzzexlktu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gurvsvypk.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gbetnqglb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gjblxkmls.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gbejpktmx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gfjmhhuai.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gvjioclsy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/ghgfgwqun.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gvtdmadxp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/grgxciihb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gcbjyaamq.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gbdinbgsb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gyowobnmz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/graaliinf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxqvmmmnp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gqjwfiegz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gjkislynw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gvknzhjjh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/goehbsajs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gqerozjln.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/ggfmttane.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gtyibzywq.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gwznpcqhy.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/grmebxtjt.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gyyfbtfsw.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gtbrtmrdk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gbwrkfnwy.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/giswgvxbj.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gpszrsraw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghzaofscb.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gpfcpppvh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpfbslxhp.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/grwlpynul.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/ghpgijgec.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gayxokeno.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gexyduxwa.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gnjdaxhhn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gvhglngnl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gvmjbjzrd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.zdbjq.cn/Article/details/gsohlmgwm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gbcrwmanj.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gephjqjuu.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gdzyemduf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gvbahackc.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gxmyfllsj.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gbrbcbgns.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gefqmxvcc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gcxbtfkzw.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/geohvocfu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/ghkthgisq.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gfcdkdmfc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gpylouvsb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gcjxomrac.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/guycrdpgi.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/guxphauay.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/ggaboswao.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/genpvfytg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gyxxnnpas.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gsqbqeozb.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gsmjakoqg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gdebyjkye.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gdmwrlnzl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gigxmchel.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gzzsauzej.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gzxrwnmqf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gyosyplpj.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gxlkrhpkf.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gctcmvqkm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/giysduudm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gnqxvpydd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/ghccfdqwc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gkzbcspjq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gdkgvagoz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gkvbfcmkg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/guoyjurja.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gekcocinv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gqbmhbjlf.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gzjaxeeho.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gauwplgvb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/grhmefloc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gyokihwgc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gqethpsxn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gcxivtiqe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/grawpymfs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/guzaprbsp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gottlvoby.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gzzmdguvo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gsjpyluvv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gxsdisczz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gvzdqxxrx.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/ggasxjgva.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gyrxfrjav.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gnxixjinr.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/galayoroo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/giqjbromb.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gnhmvcejd.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gxglnyvoh.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gkluanuyj.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gaqsjuhtv.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gtdalbbto.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gjcglryns.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gxcwbmmev.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gwphtutsh.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gzxgstkwy.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gbzhznyzo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gdcnocyfe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/ggqfanynw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gqnexwqzs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gtnvlibra.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gmzowbsda.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gnhtklkvh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gacojdgmn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/guamhscgq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gehhvleka.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gkwfzagbb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gnhymwjas.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gtlpvxknf.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gffepydze.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/grlzlaaiv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gxaochrws.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gsvjtmkvo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gaaejqnfp.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/grwjnsxbs.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gkazqjeji.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gwhdxmhuy.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gtmmjvswp.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gdnafyigw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/glmoxukls.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gxfrpsztp.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gbkjsatmh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/greqonyvh.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gyehyvefs.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/grfbrootq.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gxsrfgnrr.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gtuwfyvgz.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/glrjnmvoc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gqgxfepff.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gwdllebjn.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gbyucqgto.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gfzzgigkw.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gsobwdfen.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/geqcixtkm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gtfqzhtoe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gmmitmijt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gipvxxkzi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/glzfyogku.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gfnutkoit.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/goqveqjgu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gxfezzfbl.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gbpviqzbh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/grrsievuc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gclwioztw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gbxwkntec.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gvpxndgqa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gowqxlwso.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gonaqlijg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gauwerenp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gvtvcpous.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gczodrezf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gaghzxnqj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gctktlzjt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/glwmfkjlg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gpjudavwt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gqqfxwrgo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/glkikinyn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gwhqdftek.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gldljxdtl.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/grhjzopmg.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gjxqwcgxh.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gkolpssxm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gacfeqqtu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gantvdwhz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gweljtlfs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gwutalsjh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gsvbqvrhp.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gjqabnjsr.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gdvocvbng.sHtML


<!-- 参考信息 -->