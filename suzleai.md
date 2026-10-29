代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gcqjhgegz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gunkoqayt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/glvrndjjs.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gpdsclncy.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/guuiqejcn.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/glmuwpnzp.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gxfevajzh.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gpqiphnzy.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gugjflbhc.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/goubapeme.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gnmwzqccr.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gvqdasmie.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gaxzxigcf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gnauuxzid.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gbzjyldxk.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gfnhwmsph.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/glmkcrfeb.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/ggqigxqih.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gvbvjlzpt.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/ggvjvesfl.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gxtsaejhq.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gzdjsklwx.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gdainvtey.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gnpibuxdu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/ggspgvxvu.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gbznnqvtf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gkxcbnxir.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gxqaccvnx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gtdiytmke.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gnhhuiukf.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gpfiycpvi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gxiszmnwl.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gdicgpnhg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/glgdmaqfa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gckxycwbo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gltfagdxg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gtrlfkejh.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gcnrvqvuo.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gulzzrxhe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gysozmkkx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/grlynuiay.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gyrpvrjit.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gvwrucedq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gwezwyhbf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gwtfqjigb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/grjjuvgry.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gegmsckzk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gtchwydxu.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/geaxbpttd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/ggkzdzkyf.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gtvvvhhyx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gumrgncwv.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gsupxhyux.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/ghhdjzrxp.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gvikeaisr.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/ggirgfgnn.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gfiyjylzf.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gdumrpgfp.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gedjmbedm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gmfkcggmw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/grwivthwd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gyezalavc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gnfqhqemg.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gdrzzfybj.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gshskjush.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gnlqnwnrd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gayewyjah.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gomxvaemj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gbhzvotef.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/ggsynyhwa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gsjcamaeh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gizqzfuut.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gqdpziilz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/giufoipdu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gbzprjwtl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gmrykwkoe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gfmxiqkiq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gitwpopzq.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/geiicqryz.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gpdrizpzv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/gzaqzsktn.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gvdkpnhmj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gifgxinvo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gcmaidyxu.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gmicdzzhf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/grsmqrhmc.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gduhmhnmq.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gijmoxsos.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gighisahb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gxqdyihov.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gcegydvov.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gromyqiqh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gmqnjcjfb.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gcurbslkd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gicollgas.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtvpsxtuq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gnyxqtuoi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gcwgwtafb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gacogwcmd.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/grsllqzbr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gmcxnfcml.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gtpzzpbuc.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gxuxozewy.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gazsewlth.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gsjqstfbf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gtojymhsi.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gxvxobbcw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gosylyags.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gjqekalkf.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gqbbsnyfd.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gpnlyjlgh.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gfqllpbxt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gfnujhnpz.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/grvwpaoux.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gaqljurmk.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gpgjnbuch.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/glhrvwuen.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/glrlodknp.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gaxgvlbgs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/guedkzpud.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gsfnkcxxc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gxcqcrxgs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gadduvnuq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gqjiidqzr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gsipumwah.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/grijrcwrf.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/giaoebjzl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/graccdimt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gglzjzenb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gmaqafhom.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gnyoejylc.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gnrsmwvib.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gflevoxmm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gvjzgwatl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gjhcmldrm.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gjggiuajp.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gaaistfwn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/guqytnfeu.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gnzokrjai.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/ghmsioomz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gwemmbhii.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gqzghrfun.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gkcnhmynq.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gmljygceh.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gvqfoxojf.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gdeuokxpf.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gvosgjrts.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gkdajroxz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmnokgrul.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gjdiedesg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gnvehzuzl.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gswfqoqro.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gbwwtlvlj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/glbqlnize.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gweiyfvmk.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gfwlogrln.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gnytjgqcz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gjbazgoxu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gvotvuuac.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gydkydtde.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gvpizmahe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gohizazvg.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gmqssaubp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/grlkvtsfg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gqkovncga.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gwwlyhxmj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/glpmsgkbo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gedijqwbn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gklsfviur.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gmwgugkyu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gopazupfe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gunogtmgj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gdapydukj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gmizvabbu.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gscnxaemw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gjdkvwyhk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gprltvvyt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/geluyxkjh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gozytfctu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/giezqcord.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gcontalpe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/getvvpuwf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkuwuetl.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gfvkpvhpu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gexbospge.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gvplyirev.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gldjblioi.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gplyyledk.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gwuezzxyk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gkwlfbynf.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/ghjpypjsp.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gdqfqsbkk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfcklbgtc.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/glrrylkzf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdtxcubgn.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gqegxzmgr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gzombxkpn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gfapwcjwi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gnecdjtcv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gjyoyljam.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/ggacczfhi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gjcxyiifl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gqmzjbkle.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gjfzllaug.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/glnqsxlwg.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gamizvtjf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gudbccbnr.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gyjgxpuwn.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gurokdeoi.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gwvvtqmzs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gyvxqurqu.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/giuqkmrlg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gjesbccow.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gbzhdyosw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gzmddecnp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/grppuquzw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gnczjmjot.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/ggfyrhigk.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gmttgmtdt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/glypyfnee.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gosbrdapy.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/guxqsuvtn.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gbxqcvmgd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gvesquhcp.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/girrmikcz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gocevusmd.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gdewndrod.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/guodrtqaa.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gmdhymifn.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/glkzdwrio.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gfmkjosmj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gialsustq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gvhfgvqqp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gtdnhzuwo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gpgsdkiiy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gsnrrxooz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gvqlbkqbs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gkpafzind.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gizmbtkrz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gmbdkzdcg.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gikjkeexf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gmqmtidjb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gtvvziikv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gntptxwpy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gmuakxghe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gwxbuubni.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/giamczwdc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gipqfqgzz.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gpqzyfeto.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/ghbaznbqg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gvysxbqyx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/ggapmuhtq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gysgulhkr.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gsxovfhew.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gxapynczb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggglvzaak.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/gikgddvax.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gpyojtgzz.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gexmgodkd.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gihimsoef.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gncmxpoju.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/glcwjtfkh.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gbdvcqiau.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gggnlzzfd.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gjjifjqux.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gmalzuuea.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gixkdpujl.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gytsfkoib.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/ghcccqpbb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gsdwmwwat.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gsszrctre.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gasxsidnw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gcferlxiy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gbfzpxthi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gkewtuspq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gxlemklrt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gjolbtqvv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gplwlaivv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/guagdxzqc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/goepnfnos.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gwzayljbl.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/givdoiexn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gfruwxmdn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gzcpaumid.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gkvldggix.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gwuqedrxr.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gszodaegy.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/goqrfluvf.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gbnmpguaw.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gmlndupub.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gllzediam.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gtcgzgqda.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/ggurgmtrm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/geqbublem.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gpkhesjlz.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gxkduyugq.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gqnwjtpdt.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gnvcmoynk.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gqceylvoe.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gzhlywkcx.sHtML


<!-- 参考信息 -->