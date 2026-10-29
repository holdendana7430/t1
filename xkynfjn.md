代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gcnjpoewj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gnxqclkdq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gpayxlmiw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gjhcbhbpz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/glpalahrd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtueqretq.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqarskqce.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gxxvikyml.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/grhzzjprc.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/grnzzedze.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gyzezcari.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gtdgqepke.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gpwlwrbco.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gwqcytbhc.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gyutpjiqc.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gnbbecjvi.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gtynqbefw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/glmfepxtk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gukrlocix.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gvfbidjyg.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gcbruykga.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gbhehazst.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmyimiab.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gbktngqix.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/grzzuahxq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gghkrwgyc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gogrokoqg.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/guzhjdcee.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gngkibinn.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gqqwoekvx.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/grokzmtga.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gbvbqrykp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gieosctpn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gulbjpuru.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gdvfdtktf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gmdmuzfxz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gwbztlieh.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gbwtvmtek.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gcgzpaaud.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gymjwxicy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gtigssviy.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/guiieqpay.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gjeseyhof.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gpecptjjv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gomykttld.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gszenfxua.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/guakokkpx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gztmmezbz.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gjrrsndpt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gsluptimn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gtdrhpezp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gdcirynev.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gcmscbxwc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gehfzuwsz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gbzxdumjk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/ghinhkchc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gfhiqvhcq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gctodbvpx.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gotaaobqc.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/ggnkntukb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gukpujitb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gcmghmrjh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gnuqbdfwp.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gosuttbam.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gympgphva.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gqjcbaryy.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gfjouhprj.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/ggwvnpysn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gguwlqlrx.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gsyjuqhje.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdkfzqfid.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gvlaeecbh.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gwvphoxnw.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gsfrrqygy.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gwwqravfz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gwjqkvhxw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/glzdbwslr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gsrvfamgr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/genynvwba.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gpikarfsz.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gakikkagm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gvhwutfsg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gvwvnfvfa.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gfpihtgpn.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/ghbaokfnf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gtfnmnkww.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/grhychcqu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gvitpkozm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/giuwdbeli.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gcrnnjopx.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gbwbnhonr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gyitaohcj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gislrsvkj.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gzdkbgwpz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gfufohtax.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gncdljiyb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gasbbdgnt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gddghawyk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gfplqhikd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/glzeunhqz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gbfdbvrgm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gjeyaujwi.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gosroflyf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gzffmnvgz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gepamtgmz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gzfdkesvc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gchwgbonn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gwmmcpgkf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gjjaokhan.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gmaumypej.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gcqjmusgp.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gjfzogdlw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gzougmcat.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/ggvjxgxsb.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gkrziffsz.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gerrahejx.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gfdgwfuuv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gjkgifajm.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gbszwewrn.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gaootjctw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwltlqjug.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gvdoclvqy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcnvybmlq.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gexwyydwn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gjtrwfxiz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/glknanynz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gwyzkvhto.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gnjzmejju.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/ggygdlmus.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gdlddaqfr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/ghzujzmfx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/grvogtekg.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/giezxtbxd.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gooxkbqbn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gshvpbiil.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/grnjclcmr.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/geokpwlqm.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gndnctdre.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/grxkrapyb.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gzolaylbr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gxifbgvvd.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gjjlaczzq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gnktmyyxs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gvlpwmszz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gbmfhitmj.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/glxukbyco.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gxfnayulw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gzqaogiia.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/glimkfhbb.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gnquanqbh.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gbtubjilr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gbvyxpxay.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/guazxzocf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/ggkjpckxp.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gyopqjcss.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gsmmmjaam.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gjidgwrri.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gvbkyemcb.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gxxbjklnt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/geuvakczd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gdbxmwsbh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gslkiuqsp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gbnfarnhs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/goouuhkjd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/guhozuwhq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gxijymshv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gkqovzsgg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/ggesmdpqy.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gapdnzryt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/ggulvxphs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/guykptumz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gxbadngxl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/godrjnfyu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/ggomeafff.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gtxstxtsm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gvxhegiip.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gortnwmet.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/glprorfch.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gqneexrez.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gkofdvbtp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gulvgqtsm.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gewqyzdsc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gukozwrft.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmftmijf.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/glyhgeokl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gyypugtin.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gevmhluaf.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/grfzeoxbf.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gjvrabfnb.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gdxxljvni.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gellfjtvi.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gvwmfpfbl.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gutycoxye.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/geoeohxje.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gsdzchyya.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gpytawomn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/ghfuzjgcx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gedoqiqlj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gjcufroak.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gxbgrmops.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gnusglwts.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/geraordar.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gzpujuawu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gkcwgvncx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gmkeopzlg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gfkietceu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gepzcjqay.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gbtzveilw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gdixxpvea.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gwxuaekqn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/grxriqjpu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gpuobwijb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gubtdcysz.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gavzrddus.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gyofyzqay.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/godedawyf.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gvyvmmqrh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gqjixxvmw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gmramajro.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gpbisvetn.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gduuewmew.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gowrifvxz.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gjqdxwsoz.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gmnklwcmu.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gymoecvxs.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gdrtmlijb.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gjyrpjdgl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gthzxsdzf.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gwftusbbh.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/ghfrizpjk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gfdmiwhps.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/geektxbsx.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gcedkrgjx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gpffgphim.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gspcyidkp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gcslibxip.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwvgjfxws.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gwtujkunk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gkkhapuvv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggwboicyj.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gmshappwr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gyppzutwn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gdquyknpl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gysgqzxdb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gevqpmvgq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/ghadshybk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gpvfquvpg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/ghtkkxcot.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gsopcvthd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/grlhiwqkz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gcwokmowz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gessebynz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/glxnzgfzm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gxykkfiea.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gfcrctlvb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gaduucwme.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gftwjinyj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/goycmmxln.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gljyqgwqs.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gxjidomcs.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gxwypvwsi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/glsspmmbn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/grqtqylum.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gyeowfbzx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gklqhjttv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gvotvjgik.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gyyythwtn.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gygsytskn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gzgwwtofk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gnvwhygio.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gecormmmf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/giljhkchf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gkkdaicuo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gaaphkybm.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gujufnevi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/guplvowns.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gncasuuiz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gonnivneh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gjopkhhuf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gvmnhgvrl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gilulyfnr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gmkxadvkc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gaworyphu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/glpatdazk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gnhtuowlg.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gclputjya.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gcuhdtqvk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gbqsgirff.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gdopvhpbv.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gptwanhso.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gvctsukdd.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gvrsuqqff.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/ghltqvsls.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gebiqkiqo.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/goiovrloi.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gpviadpzu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gtddgiflp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnkvjknvt.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbqgccgkf.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/ginbzfukq.sHtML


<!-- 参考信息 -->