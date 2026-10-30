代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzibelrq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxhnvkcu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gofjbdtvz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fanxiaobao.xyz/Article/details/gcdocegsm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtphlwskx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gszkukbkt.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbpurrvs.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghngvpaex.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gleawquky.sHtML

Go:   // 手写循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcnubiow.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gbdxcbcyc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gyblekraa.sHtML

[D15] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqkyghkh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthmtdohd.sHtML

PHP:  array_unique($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gclakaxhw.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/guefsjavv.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gjndfrmez.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grunegoxg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgulzqoj.sHtML

Ruby: arr.uniq
来源：http://baike.fanxiaobao.xyz/Article/details/gbflqnmnx.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gyjtzpuui.sHtML

[D16] 求和与平均值
来源：http://read.share.fanxiaobao.xyz/Article/details/gddslpzqz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdftkcod.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvijcvzq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrtamxli.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbagomifq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fanxiaobao.xyz/Article/details/gffjahgwk.sHtML

Go:   // 手写循环累加
来源：http://www.share.fanxiaobao.xyz/Article/details/gglkyrous.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqmbrmjn.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmtouuip.sHtML

[D17] 最大值与最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gganbpcxk.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/glrsjptws.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkdjxwzu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcexvrrf.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/goudpvcok.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gobtrhscr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gluytobrz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpgrnmwe.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvenveyc.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gjytuaojj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnewpmlx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzphevtjk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fanxiaobao.xyz/Article/details/gguijmixy.sHtML

TS:   nested.flat();
来源：http://wap.fanxiaobao.xyz/Article/details/gmjvevafo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gobxtbbet.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfhybjfe.sHtML

Ruby: nested.flatten
来源：http://3g.fanxiaobao.xyz/Article/details/goczflykv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelyiaybx.sHtML

[D19] 按字段分组
来源：http://3g.fanxiaobao.xyz/Article/details/gxwewnhhi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnrwkstu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fanxiaobao.xyz/Article/details/gibeqjtbd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsywropt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gvshvphpd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznrijpip.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuaxweax.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gleupfnqf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fanxiaobao.xyz/Article/details/gewnalfds.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fanxiaobao.xyz/Article/details/gklpbsfxh.sHtML

Py:   Counter(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gtrexhlea.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcruswzin.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fanxiaobao.xyz/Article/details/glmvcvoul.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gschmxbeg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fanxiaobao.xyz/Article/details/gfucfugax.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhqnrxmt.sHtML

Ruby: arr.tally
来源：http://read.share.fanxiaobao.xyz/Article/details/gjweyrcgo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fanxiaobao.xyz/Article/details/gndxyxseo.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fanxiaobao.xyz/Article/details/gqxqeqhwr.sHtML

Py:   x in arr
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvsptlao.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbcyatiq.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcqntluh.sHtML

TS:   arr.includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqkghjgs.sHtML

Java: list.contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gibcfzhtt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/geebiemjh.sHtML

Ruby: arr.include?(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gpnwhrwzb.sHtML

C#:   list.Contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbikzpqla.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbpiaiuq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galfqzbil.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fanxiaobao.xyz/Article/details/ghntuhjxr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gfdhqbdqn.sHtML

TS:   [...arr];
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxdbjrtj.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggslpngbu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fanxiaobao.xyz/Article/details/giqcjlmpc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtcsomac.sHtML

C#:   new List<int>(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gyqyvseml.sHtML

[D23] reduce 累积计算
来源：http://mobile.fanxiaobao.xyz/Article/details/gidsgufrf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyccwgjhs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/ghnvmapor.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxlvjwhf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsflqwquu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fanxiaobao.xyz/Article/details/gufamwtwl.sHtML

Go:   // 手写循环
来源：http://baike.fanxiaobao.xyz/Article/details/gceqtzieg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fanxiaobao.xyz/Article/details/gdshpuhkw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fanxiaobao.xyz/Article/details/gkjqwuznj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzndzwsxy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gorsxenfh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvssvaema.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gruuvqrhw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwxzpafq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fanxiaobao.xyz/Article/details/gjjpfumfo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwhhmtnh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fanxiaobao.xyz/Article/details/gbnuekvgn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fanxiaobao.xyz/Article/details/gzoavuzqe.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fanxiaobao.xyz/Article/details/godkraotr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdrertmm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fanxiaobao.xyz/Article/details/gccdegghz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnndtndjc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmigefby.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaqyqmxk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fanxiaobao.xyz/Article/details/gdcvoxjnn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gtpigupoh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsgjlsmk.sHtML

[D26] 数组转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gcegzisdb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gwcaeyyta.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gdphomukh.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvgxfmje.sHtML

TS:   arr.join(", ")
来源：http://3g.fanxiaobao.xyz/Article/details/gxdszvpyq.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttsyhved.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gybowmxfy.sHtML

Ruby: arr.join(", ")
来源：http://blog.fanxiaobao.xyz/Article/details/gulcoozxj.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/glbmnenzg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grlwczwee.sHtML

E. 字符串处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubmvgodc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrdwgsgu.sHtML

[E01] 拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwfvvmqg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpgmiqts.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwyzbstg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggefxymmi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gkgubvlev.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fanxiaobao.xyz/Article/details/gzylvdpqp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fanxiaobao.xyz/Article/details/ghvjowkqn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhalssrx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnnndeft.sHtML

[E02] 重复字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gbscxjfxr.sHtML

Py:   "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/gqdgzjfqk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gxsfxnpgv.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gxbjskxvg.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuipajfj.sHtML

Java: "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gcxbpcbih.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoylbhsl.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrhrwnxr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiwpgqnr.sHtML

[E03] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gxbaikywn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvoqqwjd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glucasbpn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvffnmxqa.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumdbghmt.sHtML

Java: s.substring(1, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/gkxiisygy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvykvknoa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fanxiaobao.xyz/Article/details/gosnxcqcu.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gxtrkgsik.sHtML

[E04] 查找子串位置
来源：http://3g.fanxiaobao.xyz/Article/details/gbvohewkv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqoqdieng.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpnnzqbf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkmpjmbu.sHtML

TS:   s.indexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gnwwmjphh.sHtML

Java: s.indexOf("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuewxzpa.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fanxiaobao.xyz/Article/details/gixroakty.sHtML

Ruby: s.index("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gwabnqitm.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcgzadwk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fanxiaobao.xyz/Article/details/gitcpzfhb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginlgvlcq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fanxiaobao.xyz/Article/details/gjytuievm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvpeergz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdlvmdoq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsmwlrqp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvjewrpq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzlgskjn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwplkwijo.sHtML

[E06] 替换子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqfmjdsj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gglertzep.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzzdvvra.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrfxuycy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/grqgrkrxu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpilgmqvm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gcikppozs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gakbeyiba.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gewolxbna.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjidzgyc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fanxiaobao.xyz/Article/details/gfdvhxscv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gyqkkfwsd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gofahtdrc.sHtML

TS:   s.split(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gngnqpkam.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gelhvxkfn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnbpagcl.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fanxiaobao.xyz/Article/details/gvrhdahdk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fanxiaobao.xyz/Article/details/gnvihsqei.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzpxziju.sHtML

Py:   ",".join(items)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcrimqck.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fanxiaobao.xyz/Article/details/gafofqugw.sHtML

JS:   items.join(",")
来源：http://wap.fanxiaobao.xyz/Article/details/goddydbuj.sHtML

TS:   items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkeuobjm.sHtML

Java: String.join(",", items)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzbqboke.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fanxiaobao.xyz/Article/details/gbfwabxvw.sHtML

Ruby: items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnwmqmap.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fanxiaobao.xyz/Article/details/giqkcpcqe.sHtML

[E09] 去除所有空白字符
来源：http://3g.fanxiaobao.xyz/Article/details/ghaxrvdzu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gegmsxmcr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiwoemqb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzohaldyg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gboxfiwec.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gknuylkfq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzenrsbe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fanxiaobao.xyz/Article/details/ggtdcoeum.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcuqpvix.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fanxiaobao.xyz/Article/details/gzuqkhvgl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gshmarvak.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fanxiaobao.xyz/Article/details/grkogveii.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gdttnjbzw.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/givmngesx.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fanxiaobao.xyz/Article/details/guvktocuj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fanxiaobao.xyz/Article/details/gevybntmy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdmztgbf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdlfaxfb.sHtML

[E11] 反转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/goqbywato.sHtML

Py:   s[::-1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gicwnlhnm.sHtML

PHP:  strrev($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskxdmxyo.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwpucujv.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuxbkbgs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrwrksla.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjefktzi.sHtML

Ruby: s.reverse
来源：http://3g.fanxiaobao.xyz/Article/details/gwukdlqcr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fanxiaobao.xyz/Article/details/gdcjdcdgu.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fanxiaobao.xyz/Article/details/gkygfnmwh.sHtML

Py:   s.count("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuemsuxp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamhnrtqi.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fanxiaobao.xyz/Article/details/grohxdcdx.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fanxiaobao.xyz/Article/details/gfvndysbm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpghrbvul.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gseeopxnp.sHtML

Ruby: s.count("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrororku.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fanxiaobao.xyz/Article/details/gospkdecb.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvvyoswg.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhrrdnyo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtlbvruwn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvcuqxwm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmxngwyv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giybbqbro.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyuaplia.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciopojro.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaplwukyo.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fanxiaobao.xyz/Article/details/gjjjjmsoc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fanxiaobao.xyz/Article/details/ggvnhgoyj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gogkddatg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjmfsvji.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gxfcyacwz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fanxiaobao.xyz/Article/details/gcwlxwncv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzivnfzfo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fanxiaobao.xyz/Article/details/gkqnlesqi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwjhnlzi.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fanxiaobao.xyz/Article/details/gupervqbl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpueqiwgt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxadmffkj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gphswklgp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwtfeckz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fanxiaobao.xyz/Article/details/gmqjiatbz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gbhtyqgul.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gsenfuepf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gzaoyhffl.sHtML

[E16] 数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gmahiplpa.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fanxiaobao.xyz/Article/details/goynzeeoj.sHtML

PHP:  number_format(1234567);
来源：http://blog.fanxiaobao.xyz/Article/details/gnchtgytg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmiyjdfs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyevbzmq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvopudvxb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fanxiaobao.xyz/Article/details/ghaizhcmb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwosvsym.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjqtbfhf.sHtML

[E17] 首字母大写
来源：http://blog.fanxiaobao.xyz/Article/details/grycjbwbe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fanxiaobao.xyz/Article/details/gboqobwae.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gmuyehmiu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gtptztmjk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxouqoct.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gujulbudm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gkepcoxxn.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxnpywwt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fanxiaobao.xyz/Article/details/gsuvwmbmr.sHtML

[E18] 模板占位符替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbtmpbqjs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fanxiaobao.xyz/Article/details/gujmrvtho.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamqdellx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gzyntxltr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gacegfnth.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuznhvkq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gghroccvb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzdijgae.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsxhpuxb.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fanxiaobao.xyz/Article/details/gjyycatjj.sHtML

Py:   s.splitlines()
来源：http://baike.fanxiaobao.xyz/Article/details/gujwtfhxd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/ggtikyris.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fanxiaobao.xyz/Article/details/grlsfgtqy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gahazhnjg.sHtML

Java: s.lines().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpghsapk.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gcpcyeqny.sHtML

Ruby: s.lines
来源：http://blog.fanxiaobao.xyz/Article/details/gmlccuiwv.sHtML

C#:   s.Split('\n')
来源：http://blog.fanxiaobao.xyz/Article/details/gwlqfzmri.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihvowgzv.sHtML

Py:   if not s:
来源：http://www.blog.fanxiaobao.xyz/Article/details/guimpjrln.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fanxiaobao.xyz/Article/details/grqnhyega.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gkglqgdhv.sHtML

TS:   if (s === "") {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbeqsgdxd.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxqucbdi.sHtML


<!-- 参考信息 -->