代发 wailian999

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/goxnczsln.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gcvgqgpfw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/getymfrmc.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/glkxwjroz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ggxjmmqfg.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gkwkbnemi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gkvtuuevk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gbuyraeaa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gobxysgca.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gxvrfivpy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gbagzshcp.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/golrtbzrl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/geekcdsur.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gkcqpuojg.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gfkssircb.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/ghgsgodvz.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gtlrzovwb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gjxkzedpu.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gykfujlln.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gdghvcmxj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/ggafryhbj.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gljjwcrdz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/guzqtxjyw.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gwbmvsiez.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/glghsxpdj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gvpvecftl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gyqjoquts.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/geoxvouxo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gryyfpein.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gdqcgvuyq.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gfloldfqz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gwhbqmlsu.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gzcpoxpka.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gvvrqcveg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gheubzedp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/ghphfjjxf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/glmlcyidh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/genohbqnu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gkqbdpuis.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/ghtvgnrqs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/ghobbzzdt.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/guxbkghxa.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gxgrmjpoa.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gfcqhsujr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gbyipxxjl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gzsypoefi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gsvujvmha.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gwkznphed.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/ganhgbswe.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gfxhjzfaf.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gmcmfixif.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gzrkjabbg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/glyvyshhu.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gmxtrvnbx.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gvhnytfjp.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdofhtsc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/goxprhmxu.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/grqijnmvy.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gcyelxrts.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/guzsqhepd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gcvdqwzth.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gkqapyokg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gspfyemtl.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gbvipckey.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gilfkkcxa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gxjnhwkik.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gntzzogxt.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gtjlsjdfa.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/guguvbhah.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gmkwpvlsu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/ggwwjmnav.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gxqhibyse.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gygzpylmo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gedqsoacn.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gpxyyvzvo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/ghsarujgi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gbyuwuqge.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gpopqanba.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/ganqhiycz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/giuhjhskr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gabrvltov.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gfgmrmwce.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gxwfqfxiu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gjgmxttwk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gddzjiord.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/grybrqrks.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gfkmqejun.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gxghymlvh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gtjkafdep.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdanstffs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gbuwexdux.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gxblwwpgj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gaqnkytix.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gveqzlope.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gzcrofxld.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gheudulrg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/goedypvim.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gyyjgpkqu.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gummujtgj.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/ghsevaclu.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/guhixdqez.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gupbzfoou.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/ghwdiyzkv.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/glwlbwcco.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpxlpqbat.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gieejdseq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghqstdlop.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gcqlxvzsn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gvafqoegv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/ghxlwfets.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gfjafttxa.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gjaxyjiug.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/grottrjjq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gdmktnamy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gteymezch.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gozksratw.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gopqsayal.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gbrupfvgj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gcrgvkzms.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gzovgxgns.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gkdzpnjxq.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gkvyajdlr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gtueywuha.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gvvmdzfne.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gzzawbwpy.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gtuloksfa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gesprpivg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/ghllqcrmd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/grfyefkuo.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gcgbxtvow.sHtML

Java: s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gjpkrzezm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/getkhesfv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gjyyemvxp.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gszimwjsy.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gvavdrepu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gyxhjrswr.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gkdazrtkl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gskvynfej.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gnszqkkff.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gtsdsqsbu.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/grwjbfzlp.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gjmegdkxv.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gxyztwhmg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gzjbyqeah.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gpdodaqvx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gzjpaywfp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gpwgeeurf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gxybqxfmz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gabxwpjci.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gwuhxobdo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gyhjgbver.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gjixflkwz.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gkjugjzsf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gppimkuae.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gbazwygnv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gplrshkso.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gygucrmsy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gbxgbmwux.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gesfcumhi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gugjxjege.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gpercauyj.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/ggltubksc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/grntkkoma.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gpdjrgksk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gqcbccscd.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gdwezpiaq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gjwqjycnn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gcpcrvqak.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gzxlvdjfv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gkbtfwuzz.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/grnbcmtur.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gukvayzti.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/ghmbqfypd.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gwksfbwti.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gelgufatv.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gxnqetfbh.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gjjqlvywq.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gcgdtzijd.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/ggmcbzzgx.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gdfuutkmj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gutadxnhz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/glnijlyaz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gfbfadthl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gshjcefun.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/guslipqnt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gyfcqfjpl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gnvtqihse.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/grbcuodon.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gzltkltwu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gyrnisvfm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gspobnssv.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/glearhxil.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gbnsczuma.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gusigciin.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gaozlotea.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gnfruioln.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gajruaalc.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjzmfduac.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/geznwrsbi.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/ghvahjmiq.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gpmlumvbp.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/giifyahzb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/guqgyuwaf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gkptjrboe.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gqdxqidrd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gkiunyvmt.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gdedscyow.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gcbmeagcq.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gdgeqeply.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gqwjalraz.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/grgmeexmo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gmczoriog.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gghvxcnlt.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gwzttfjdj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/glqhodgbu.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gntabelxz.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gbenqajlb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gvogsaaoq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gemrohrma.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gepkkrbpp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gtfbketze.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/geepgyuqs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/glqyqqmlr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjrvzxcdb.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gjhpcthui.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gotwkpwsp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gyxknskff.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gqqkqxedc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/glvnkhyya.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gpqwtessl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/ggukvjoae.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gbaezhksg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gnlfdvczy.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gduqirdfo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gbqeaopjs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gexvjqrbx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmfznlqct.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/geewavdpl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/guojruqhz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gaxveempm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/galhckuyh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gfipesuim.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gjogwnlkk.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gqecymahy.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gplbnfrrb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gitxcaoaj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gpyocoxwc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gvtsnfsel.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gfjqbrozb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gcjttuspo.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gewdzdaoy.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gkwgjqwzy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gyvwdhzop.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gyxbvayid.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gsyrjcbga.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gogbvhpjb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gphfutcua.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gfvlyylle.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gszouspde.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gbaikdkoc.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gmruknsrq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gbsdqgqtq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/ghitclwad.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gejzslpuu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/grpillpzm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/ggitzmlws.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gdkeywglr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/glfvcnrur.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gyrxgumcf.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gkkxduwiy.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gkuwtkoma.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/guvazblrk.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gmfyimpjg.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gymzbwozj.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gymlefywx.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gpymignli.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gyuawnhvx.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gxszhwwzr.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gffilbfcj.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/goeafeeie.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gapguulhi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gimixmpde.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/goujnfwnj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gjdpvdxqm.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gbysudhse.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gtsfuqxyk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gilrzpigb.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gckihbipn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gqmqkcthm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gpamhtivs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gzjujgxoa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gimavxvwj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gxoxkvoly.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gxpemunjk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gpqtcvgkp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gtsklmujk.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/glzzuyuny.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gxryaobmn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gcqkgvgls.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gdhepdesc.sHtML


<!-- 参考信息 -->