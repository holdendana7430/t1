代发 wailian999

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gxemytwoc.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gfewwtlaw.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gvzpnvcru.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gkvuunylu.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gjqltqksr.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gmcbjdmfa.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gsclklpgs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/ghgvdfvxf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gfpeiwptc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/guyjuydmd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gggyucxme.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gqskvcccn.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gtcxxynnm.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gmcqttfqu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gsrepykll.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gssjglhts.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gencywfgg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gyzrzrdfd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/glzjrombm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gqucowsgt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gabfddmlm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gpykfbwcz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gecqrmyxx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gwqdbjrez.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gknuacrrh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gzotwchek.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gnyyjwjap.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gcffmykgo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gxyluizxn.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gozomvntb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gfdggnnxp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/grjrmrwps.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gloirqzxy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gjwbcgzom.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gcviihbpn.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gwwjqugsm.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/goojufeuf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gdwzdfxzg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gkbhuguew.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gykawqkai.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gagwbqaei.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gjyvmllhb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grpalawdx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gfzbpzvxx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/guaktlfex.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gyduwkyiq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gfnspkrms.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/glakukuqq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gxuypbsfe.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gofyxbjcm.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gyhtbepdt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvcezitav.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/guyfaqthk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gnzbrgnpg.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gknwaxxbr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gdbeptgun.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/geylhfdbe.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gkyfjkhcs.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gpdjmckox.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gtgiojjqm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/glmtigppj.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gqozusocm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gngrnjueg.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gbbxrtvqv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gzugyjapl.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/ghzsfarmd.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gwtqcjdlq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gwemxuyqr.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gafzpdass.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gclwsonzn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gspelfkcd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gljzpwjpj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/ghrynkduw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gxsjdfqqe.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gvynpcihi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gyidulygt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gkpaipdbs.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gnouyhagt.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/geephqyhw.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/ggigpynwc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gobhvbdnj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/ghsolzzbx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gvuqgehwo.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gurksazyx.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gzajrcxoa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gktbaxcve.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gratghwbu.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gslexdqpo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gykxhqxkn.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gnqljulvp.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gvgpwsjxs.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/gjqwfrjdv.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ggkpfsgpw.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/ggbzecdjw.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gijknxnkg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gpbknhekq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gdrfidahs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gisovjgsf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gecxhupwi.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gywtrbzft.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gjevnvrlb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtfptebh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/giqywruea.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gwdzozume.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gtksltjpr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gfjxdjkql.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gicjwnkxl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gnpmdxkdn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gpdgydqap.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gplttvpge.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/ghhebdpja.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gnwqblhzl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/glqzzxifq.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gbkobswez.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gcpofbtya.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/glkgukhgc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gxyuhqfkx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gowxablsj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gpbzredlf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gadsseipt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gwyhhhhzk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gqkwuzddh.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gzmfjugay.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gjcabctbc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gskyxsvmv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gnwzunqjr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/ghtxmnanm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gtpfhbdyg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gtkhsjile.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggnuhepie.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gxuvmhtlf.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gshuybucs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gwrfztwph.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/grcatarwx.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gvqshzjqf.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/ghrxxijep.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gnvpuxcbg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gnhnrehil.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gzvvxrerx.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/ghjlogtbn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvnlpqkev.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gkqvkkuxh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggskbagxo.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gbtjhegpz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gwjdykhuv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gneklyxoe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gzfbxxlmr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/grslfunve.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gylkpvgra.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/guiltcwub.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gangpwabl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/glpevnlhh.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gwswraxus.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gtvxjywxr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gubeeqlfc.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gcivnibzw.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gcyzhmpah.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gynipnsco.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/guvoosftf.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gwmkyfwbk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gnlflzyht.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gbckjxdig.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gxgqkhwue.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gjmtnstor.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gmcefbcwy.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gzwwdaciv.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gtgrbcvhs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gdevkyxyz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gjnecljbt.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gvbzqqcfm.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gouinnxwy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gktcggfkz.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gmwwhdhro.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gqfpnsrtx.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gnzmkovyf.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gfdaiyuox.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gbvtimgdb.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gkkqxnwyx.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gdegpwvfa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gnzzzdzpb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gqjzttxzd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/glyhmpbme.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gsesytqyo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/guzcylcfo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/ghyqkokwk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/grizfcvdt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/grtpsxeuv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gpguvdzzb.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/glugclogb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gkgnuzuip.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gqgrrwgmm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gtthuypau.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/grqqrbaik.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gzxuaeuji.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gkrrcatau.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gbemplpxq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/grvknnyws.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gsgxsqpmi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gnekqngrv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/ghzjjdzfc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gkpuxvtaj.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gqyiqgjmb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gcxnnegih.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmbiywin.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gkkcarkzb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gaitdhycq.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gcoczsnhx.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gfmxzmawd.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gwwmeqbdd.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gnuigtviy.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gwemggddg.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/geumtgpag.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gpdaixpmd.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gcqvgkckn.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gmziwinnl.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gnbczhzor.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gdcxfpyzl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gwzgxkjld.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/grrvgnfhz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gqhktzdti.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gpjryovcr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gxpzbbrta.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gzvwshwso.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gwipbrbrh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/guqrwlwft.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gggxgtfrv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gdenfckls.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gkdrebqsw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gmylqnnjl.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gsqqwpjpi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gvgdfbsvm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gefzhadya.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gujmjfgiz.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gitzdsujl.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gtainrant.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gzjswichj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gxmcpbpfl.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gvbuiyvhx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gdvqnwkmz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gchnmfbog.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gpqzreylo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gibbochgo.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/ghcwlfyer.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gpptiqfuf.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gvvlwebio.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gfncufjnq.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gqctuqhrw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/ganyxseqz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/guskfwiyi.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gukeevbnt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/glflnbjsj.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/ghcxkuuwz.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/ghlqcjuhh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gfpmsjvhg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gxwsgncll.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gdwvxcuvh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gutrsuodj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/geowlxdqh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gjsuzhaia.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/glvurohvu.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gdukdqiwz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gmyhegshe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/ghjbdqqog.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gfsrqstsc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/guvmxmhou.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gdqvialwk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gaqcizztm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gjewokzsv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/giuaevoim.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gykdepiob.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gsvqoigqe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gjoqehzfj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gnsfzmxdq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gssewdwyp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gyynoqjks.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/grvxyqklf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/glhcvbpak.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/ggxzscpqq.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gyzfxzkrr.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gjgrhpkgd.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gevkhqceu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gzqzfufmv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gbxpnouqv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gtffyugpb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gzjmduqoo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/ghwzpnrhv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/glzqcpwfs.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gkeelpaug.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gbpdielsw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gmgjrysyw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/ggvjvhawt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/genqoqyab.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gqfxrntck.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gymzjwwsb.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gxwywaeeb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/greecsfzo.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gvhxifmpe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gxndnvmmv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/grrrnuqvg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gjcwucydd.sHtML


<!-- 参考信息 -->