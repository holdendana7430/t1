代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gkpyldxse.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/guaxoodxh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/ggquwdjpa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gjhrhliet.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gcnlhcyou.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gwndnpkdv.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/graesyecu.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gnfooniyb.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gijhiuetn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/guowfnjbt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gcwikbtax.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gneddcetq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/ggnjdnosw.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gpxajmryr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqyzikxd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gnzfejhbl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gxppvgkaq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gsxmqkadu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gdnbzczzd.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gsauqukvg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/ggqdrtcuq.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gmqpvjqhq.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gunheqqdj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtembamfa.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gvpdxdggt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gtrbmwnfm.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gyhfsoaas.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gpgbyvovd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/ggvvuueel.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gynlhzuxk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gzhnqeyjw.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gmrnjniqd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gqiobflei.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/giesapizr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gdamazttx.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gmruzqrrd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gvyvjwufi.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gbrdpanys.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gtiuauafq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gotxbxoai.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gfxnjiblj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gweltorzf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/ggnahzbmm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/grwncityk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gczilqoff.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gfyvkpowu.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gaoppcxul.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gzsgzkebl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gxabypcvy.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gyjivoryk.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gefcqnczv.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gzwscudvz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/ggvzbcsjm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gmeelwoms.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gyhyucdjg.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gpemtimkp.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gynrijifs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gpnzquaih.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gsqzehdbm.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gauztsnql.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gblspgaew.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/glhtjoowi.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gptcaxdjl.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gofzyddlp.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gzqzbdjih.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gnvjiekdd.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gdjtadxdo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gyssaofau.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gatolugco.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gxoqtbwci.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkezsbwvj.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gwbxiecgd.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gjqcwtmcg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gmqkstlvq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gscnuigkr.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gjepksnyo.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gewynmzdg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gspjzzbhj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gmzgwrhrl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gjaxaegdj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gutwrmapz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/grofpditi.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gvodhppzj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gthmeimfs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/grfrwfkzf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gdztxejte.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gnptxwpad.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gkvscbzlg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/glehigpdm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ghqxgdgwm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gilmozfur.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gnymwfnxl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gdxsxdytb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/ghcdxzyec.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gykchuydf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gkqlxwzbx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/ggnbkcycf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gdgufknmw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gskoutwop.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grvniiebt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/glytjykca.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/guimgxfwl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/ggbeirgfq.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gokgttymz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gvxcvkebj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gxwlxpqea.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/grentmzub.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/grurjmyxd.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gewrjcdyv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gejjwlnhf.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gcmzihrnq.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gitmwwfri.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcixsjznx.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gsapkbico.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfwspnxpl.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gxlgiemmi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gqjlxaokx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ghvswzqfx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/glldahvtz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gcyhmpnyt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gefxrslnz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/glwocdypm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gqqcharfl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gjequwjay.sHtML

[E02] 重复字符串
来源：http://3g.fehbvm.com/Article/details/gapfkjvhm.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gaaurimfk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gpfakeyqa.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gsqmrtvhd.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gerxypvmj.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/ggaokfmaj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gaaejltil.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gkicujmmd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gfxouiykd.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/ggpsvsegi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gxoqffymx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gysuefmbh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gcoxrenxc.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gheefkxhw.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gfznndimo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gnqerrgfe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/geutevkcj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gbryfgcss.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gdlvdqqfj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gfrfspwwk.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/guqrujgrf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gvbllqejz.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/ggpvdsfis.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gxollhldm.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gjyteiorl.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gydaxarkc.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/goywwtiqo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/goppsslzi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gwzyksift.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gaxdatuak.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/ghwkhpjkp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gjtevrgqv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gfccqwqzi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/ggzebgggi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gfhosldzh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gfpyoyyho.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gvhbffkjr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/glutprbal.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gxywzvnfa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gihuuousf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gfwjnslqv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gtgewbkkl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/grjceeaqa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gjmjztbjv.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gdluwkwlr.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gvpdqagsn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gmggtnojy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gzwlcitlj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gjnxuccsw.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gmetkwtgs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gcdsrlsox.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gblzsjvrv.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/ggebfehvr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/geemtnbln.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gaombkvzn.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gbegsxulr.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/grnfwtyeq.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gpnswdwru.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gbhwadyac.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/grzuxkdsr.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gtdxpjgmx.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gwnmavlwg.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gxqnvfqxa.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gxtheumww.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gigtzchnj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gljaklwyw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gmojlspfl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gwafiloig.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gryrbeuyl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gzaghdjfg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gsbfjtwgl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/guklunewt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gowrdbcis.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/ggyvdotez.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gfalpercl.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gstalzfod.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gwfbicwqc.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gnqlxogxy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gaqrzoqfj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gdbuiqigi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gmmtkccld.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gllsizoml.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gcpanxkgi.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gortuqjlf.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gopchwnhc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/ghddxfheb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gwowzhnbv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gpeprcdxi.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gnmlosbsp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gtyqlwmlq.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gbyvhxxso.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/ggedacruj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gfuvsxqep.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gntootxaa.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gnyvqudwi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/geenorgya.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gcdtutich.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gzkijnfyp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gatvxzalj.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gahashuwg.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gllrmbsxy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gnfidtblv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gvojbdhoq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gziivcgbq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gsflhxlut.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gunvhmmdh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gsxenllnc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/glsafacqn.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/ghazsmhcn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gzixunixl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gpomyklpb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gwsbhqnyt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnbetmtek.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gfmiuhmhx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gckwzcqqi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gwdzdgors.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gfxmupvjn.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gikuguyvn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gppfaefrv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gzbgxcnis.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gvbkoacxn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/ghxzfhmyp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gqscibedu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/ghwlyuauq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/goxgfzsqp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxssputa.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gvifsjqux.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gzqxkkxcx.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gehatfjsp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gxkcnqwwg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gyvkawdmy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gfabuefxz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/ggxfpygio.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gureiqwls.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gungguapq.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gtfiwfisc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gvdpjlnpw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gpkiszgjs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gccclgtky.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/glayujjxh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gnbgdbyna.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/grwvunbez.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gohbtymmi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gnfrnidvc.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gdbltfpvc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gsqaujfne.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gcfdwgadn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gxroecncc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gmxfinqql.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gvzhrgspo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gbfghzjpe.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gbgfsedcw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gumrgjhxd.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gtnwtuwmy.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gmydtlnyl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gkpwggnjs.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gblvqvyts.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gfcsfrmvt.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gzhtjdsuj.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gxynrrhuh.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/ggxufvosr.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gkjsvnoxz.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gsjdsawxp.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gvfivxxkj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gknhjbavo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gvsinwwig.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gwfoxniar.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggnyhtzxz.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gbyiepfht.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gbhornwpo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gnuxbpyln.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gkxurmlfc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gvomdnvbr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gfrbchdyc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gkzfjdeae.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gqqfyiawh.sHtML


<!-- 参考信息 -->