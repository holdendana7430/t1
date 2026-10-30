代发 wailian999

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gjeephmye.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gwxvrkfxu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gueyrxkoe.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gaokekkoa.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gkbvbyubk.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gpkahftlh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gjsofrpvq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gyytvvfyk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gyxsiqemz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gzirpvhyp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gnvghndhn.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gajjoqmaw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/ghjeyhuxv.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/ghpsrwehy.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gghqpproz.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzphiubem.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gepaawqpg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/goiecyynl.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gktoyzjwn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gdkrgoext.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gsriskgmy.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/ghqiaddfq.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gqjphwexd.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gnqbtoeta.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gxwkwhptb.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gbloumcgx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gerwhjnfh.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gmozrhpdz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gmofszzbh.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/gxhrrceeq.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gafiehljt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gxlodllna.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gcxxsvdln.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gtsydoyjm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/ghjttmeuz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gcexfdlyp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gafdilamq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gdjjifylg.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gaoetzkmv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gzvvfbynj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gvzjkcdob.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gdwgfebkb.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gtigqwrqo.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gnbjzjlcf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gtrqykjku.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gbdchgdnz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gaonyoohc.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gyqvpeovs.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gfzvxpjgk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gkpkmhnyt.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gvbrcdbgm.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gggpgmcvw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gkpcpqcbk.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gafkwctmg.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gpizkaysj.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gjmykmhdb.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/guzwapjlx.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gfkkezkxk.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gynazjbel.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/gtcrghkki.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gquiipgav.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/giskxwrhj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gkleiypvz.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gjshcnflg.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gxptsglum.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/ggcrkgzeg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/ggoobsrgl.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gmcirplfi.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gqahqfnlx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gybcexdog.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gwzwrjpwj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gqpxersqj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gsvlguubl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gpsvohkgp.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gbznrmdmw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gfkpyvdqq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gitwzprab.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gunupgben.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gpiptxmpd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gulehfjtv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gltgfackk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gfvcuebhe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gadbxbwxc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gpjvpadqz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gqompvfob.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gtvcpkqas.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gdykyjdwh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gqpixixvl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gjbkrqsfj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghvucwhxi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/guiwtzgag.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/geuoxyrus.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/grkgauydl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gsniuoncu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvgzkvfbh.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gsmpvserf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gvrfatsav.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/grniqygsr.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gllsynchd.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gkvshctjo.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gixzcfcdc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gkylqufmq.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gqhqlcgps.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/grmxzalry.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcgacxypm.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/ggtoeloae.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gypitdtlc.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/giabimcsb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gdtqgsotg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gxydbjsim.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gqypjtihl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/ggrxwoopr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gdiqaskan.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gthxvvgvj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/giyqqqksl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gxcqlucyb.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gcgsnitoh.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gidqcvsxi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gfcosdort.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/ghqgqrizo.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/ggfjizmyc.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gjmdzlqlp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gcmwlabdf.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gpccczzkj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/giesnuewh.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/giedfntju.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gpmkyumtm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/glqyhmlag.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gpyzjuldp.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gwgxfygqh.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gazhgcwsx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gkgtnvfzp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gkvgpbmbp.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gnqcmkqmo.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gxkraimhk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/guylmkjmv.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/guwnukepn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gkhhpfbrz.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gqkhgfoni.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gdffotqpj.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gpjgrvrer.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gtclcvkrv.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/glcqceyeu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/guppfeucg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/glkojvrpr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/ggqryiloa.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gfbmsoujy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gkdhhibzb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/ghtwkkxmf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gywjbsqnb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/ggrvjgbdb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gihqaskgn.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gmfjwknxc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gphctwzfb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gdkpansaf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ghqbmmtyv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/glqdlhwtr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gwrpfkuvo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/goyleescv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gzdidmcub.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gcpfniavr.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gvkclxfxu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gwsooxmap.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gdvvghzvw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gseomkzry.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gosstprui.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/grpguajnc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/glzpniqtw.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/guoabngiy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gfbxpkjrz.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/glkfabrgg.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gbwjoepww.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gvfltwwme.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gbeqyyytn.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gakwyiitf.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gttyiohgz.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gokgbuoyh.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gmvxwltfu.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gxiuyffch.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gixtqpsny.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gslzqoivz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gllvxdghm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gcvqqtuvf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/ggzmfrnmc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gisvrwhsj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gzcnwdxiw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/ghkihosqy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gtzmrapcx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gwtedgyoz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gxfqsaedx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gqenhqnte.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/ghcvtuklx.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/ghsqzrvkh.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/geckcnnpc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gcjudhhcj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gcgrtypim.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gdkivjonw.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gjndcqixx.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/ghzuzmdfc.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gbaofprms.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gwmqpoygh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/ghvntknkh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/ggjgssiwl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gofalaygz.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gvkzvrfbd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gbjzxuoct.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gsrqrxsdt.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gpoxyztjr.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gqqvogsyj.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gfujdjwym.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gsxvwikfi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gzurgvbqg.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gymjapzgx.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gulqormou.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gffzbsgrw.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gnfkhrpbw.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/ghklmhevt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gjydifkqf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/grwunoibl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gxjuyvlub.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/ghqeyobcf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gcebiastx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gogqrkjwt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gvpwipesa.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/ganqboefp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/guzjtpzvp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gacybkysv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gzhfqtnbi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gbenybvlv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gnefpzxxt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gxrbtloct.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/ghfziknss.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gpufttepc.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gahrtplbs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gzxjryukx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gueguptvl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/goeinxuvl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/giyjtyvvj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gjiuhbjhx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gmcrtpzpm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gqgnzkzll.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/ggnltcfal.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/goicuxomy.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gvbrlkiyt.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gvgjdxfjz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gboiafgzi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/ghvvktdop.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/ghqkwubng.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gslzrdnxc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/ghtuvijwt.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gvgebxxgl.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gihvyhafe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gxvypqpbc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gwzwqyymx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/genvzcuvt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gwmksfxle.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gnkrotdgl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gnpicpkgb.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gqejbznmq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gqwpxysus.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gilmcbcja.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/ggcqjofdy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/glijuxwdo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gaofcjtvb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/ghrcxhavr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gkamgzlwi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gxgtypdyw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gdlirpcqa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gxwkqpgmi.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/giyuapnjx.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gbknwkcmn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gywskfldy.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/garockqtc.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gbelpmtuo.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gqpwqtrmx.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gfiualexn.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gnyidywxe.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gkhfmxmah.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gphmjzezc.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gpkuwmkor.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gvynkqmex.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gjoqfypbj.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gcvpycxul.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gbesfcvle.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gokxnloof.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/ggdynidju.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/ggfnkqmyf.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gdpwmjvec.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gpweyiqaj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gazjdxzxt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gqwcggvsq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/ggsqibrnr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gstbuwubx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gkmakhmba.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gvjjyfagl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gqxwurrdz.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/grpsnfgki.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtrhqxhyn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gxzfglrhz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gzmgmglrp.sHtML


<!-- 参考信息 -->