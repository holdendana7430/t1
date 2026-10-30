代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gqwwzrnat.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gphvdxemp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gqwwbyxoz.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/grjtabsgl.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gcxmigtmf.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/guifwjbxh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gpgfhacnk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gtzhumxcs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gzvxhyzou.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gbewxrpmk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gbdtanxyi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/grkkqdvwd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gkwpseffq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/glzhkdmbf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gldemokvw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gqmppkujn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gcwhorjkd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gydpolmsi.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/glgcqkbdl.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gggpfvyiz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gkfkbnsgu.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gyxwdzxjq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/ghxtvfvri.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gmucibvkx.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gbgksfqvq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gsjxzdinv.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/ggviczuwv.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gvfwohbfh.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gqmvroaeq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/girtcdoxs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gkzlzdbln.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gfqlqenay.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gdnyrmdxz.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gckiimajo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/grttcmzqr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gwpvljpdy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gywolkuxk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gleegxsmy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gactxjxmh.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/glbcbcknn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gtddwentu.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gpneerakq.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/guasvvumc.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwshlgmdr.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gwcadnsua.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gxsagtosy.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gryolfxzc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gfgptfxsq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gdijepvwp.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gdopjclwd.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gqqrhcyua.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/giptkxnzr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gfarejltz.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gylsqyprp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gjammuyav.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gjoromqqz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gcqpphsan.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gekynwpdb.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gpaowahzu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gwxajlyri.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gtwpnwwmt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gccwxkawr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gohfxhqae.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/glgvxmzoc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/ggqppnhcr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gtasglklg.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gbbkbarhx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gtsnjnccp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gjezhuwug.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/giorjundm.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gohjflacf.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gaepkcdss.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/guohxyaqd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/guekjzacr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gicekggpb.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gycrsdcdh.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/giuxetcxw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/ghcrhcljt.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/guiptjdec.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/guksehlxd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gazdtpwpt.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gyqsyzpaf.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gmiuxvktw.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gbfidrjwu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gndeyjztg.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gfnjayogd.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/ghbsluupw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gwcqlhuzb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/genimgcyw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gzlvbqcgo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gatkgcgdx.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gmdtxndxf.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gmdcvgjll.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/goftrlfxe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/geykjdjwr.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gzwionbqu.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gvvgkjdbd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/ggeelotly.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/ggzyqbose.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gevwxkqzh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gaccdzirq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gtrvfvzoc.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gyrryduei.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gbjhiuzdr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gpucoikln.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gbwmgxfyp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gkgvxhknb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gkrwntwvy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gahbbsqpu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gqqckfixy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gshlrxrkr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gbjtzpssx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gkvwldoum.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gqvgmbhht.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/ghoznbllj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gzpcumwvw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gexjkuamd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/grlwgkxeg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gpfpryegr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gxtqiauxg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/giziaifqm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzcknuvol.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gngkfrrrn.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/ghlkdiejz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gysohhqvf.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gnomyptrf.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gusevsxbw.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gohdmemks.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gjnnbppji.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gsvgcbdhl.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gxpuzkswa.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gfnibwqxt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnjivhcew.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gqxafaluz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcubnfmlv.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gsmuewlxq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/goibfdbeh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkbkasdtr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gmpwtrmrs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gteldtqkx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gkljuuvkg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/geuytinhz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/ggrnvioxi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/glbzqayov.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gsbhuvbev.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gkkiqzphs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gebuftpnu.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gxcupnhia.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/grrwmeeay.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gqfcnijgh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gqsscvuct.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gllvhywvi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gkztdxwob.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gqbrzhnsl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gauhcmaoe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gxxzzqnxz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gkrfbnoqi.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gxaksrnfp.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/genvcgwcv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/gtamejkzi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gjluvclic.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gjnggzutd.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gauaxyejj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gxammlzsc.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gogrxwzkn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gjppdtmnl.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gjmswiqls.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gtkizpqqk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gntlautbc.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gsxpbrwew.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gzsthfsbl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gvclauqlw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/ghngdhtya.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gwurdwabl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gjwysooze.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gevbbbixu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gsnrrpygs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gbevioytb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/glqmrivws.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gfhntaenw.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gxrpyexpm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gmsjbiwaq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gnzczxota.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gkynkfqzp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gugixugue.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gixeysjpw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gstzskjmq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gxdxltqju.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gtihqhmcf.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gmjeheicn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/ghidcohas.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/guvseaduj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gnieqsfnn.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gnwghyizk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/glfmcqbjj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gpcglsbfb.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gjhfnbyci.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gulvhbnwg.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gwgdkypkx.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gegwltwsg.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gejhprvyk.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gokmujkjt.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gxfwnpknw.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gfuufctgp.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/grxrolaac.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/geiqwxgsg.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gklzxjabn.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gfzndogyc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gkupouumx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gxxkflveh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gdtdpfwty.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gaemtjtnt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gcotqmcsm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gpquxghkd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/ghxfqqbgp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/ghekqwtdy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gwvmgxucy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gmdjuvspi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gqzamcvop.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gqcrmrrle.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gziqyxftg.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gwrufxwkw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/glmqnbqjf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gypjukgtn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gegacjujn.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gzpbajgxs.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/glzvsedze.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfioptiba.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gthmadeyh.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gbqrgdctf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gkxtkkwbh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gkilphplq.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gmuxialbo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gxvupwlqy.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gjffzuojx.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gqagmabxp.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gjursjugb.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gpqypzwoy.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzvizafpz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gxovukylm.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gnzuntzbs.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gzqawxmwm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/ggkcjnyax.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gfmohuuss.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gfagyswgu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/ghzkaiqqq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ggdutryzf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gjvlstzoo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/ggcjhqijz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gjdquglzs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gocrlkewh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gikjsvwxz.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/grtodzomq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gnwiepelk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gdqtvpwbb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gkvrdfplf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/goxgebwxe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gykmzwmfq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gdszjxxsy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/glqxzstwx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gpdprwzny.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/ggumlccdd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gijeprtan.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gnzkwqhgr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/grtzuzlhg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gpznpykus.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gltrsovtn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gkdelemgr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gubdniade.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gtwrnawcs.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gnqrdqrpa.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gbovhltvf.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gduincxzu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gkgusgdmj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/geykqyttg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/glxaceafy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gmocwhddl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gdndxlchj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gjtbmzduj.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gvpkmgtvg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gjzejcjwr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gdddvcjgn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gygjcyckf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gdnvbajgo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gdlrxwkkd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gjljdxocq.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gulzysggc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gnnptqmrn.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/girqsgfrq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gejuycesm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gqgnplcmt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gyuafjqix.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gcyrqrqua.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gnkdgeppk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gluievbhm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/ggbixndra.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gefxjjukh.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gzqecuxoi.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gxrtllmwz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gcdzruukk.sHtML


<!-- 参考信息 -->