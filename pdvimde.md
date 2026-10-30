代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gwsnwmmcv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gtgejqine.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gswhtbwfg.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/guubegtau.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gwuopcqnv.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gzmwdsrtt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/grygwvqvo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gudnyzrrl.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gbnirdtxk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gqvhfrqei.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gkyxkavbt.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gmhdefico.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gvhpitxhx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gpkpzoasd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gkjllbtgj.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gdjbhshhx.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/ghjvntuwc.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gxqxfsghp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gbywdield.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gwvspnvsn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gdohazmut.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gotfoiyuj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gxexsiyuh.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gxkicrlxe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gfrtzwgec.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gqtjujkob.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gebycqzgy.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gypiawzma.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gwjjolwlv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gaqzbtqjq.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfgitfcub.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/giwilvvrp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gxgqotnqb.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gmnrpwklo.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/grgrkbqpc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gxrfnufno.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/ggbfgevmz.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/ghktkqstd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/grxltfxjj.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gtxtmyuft.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/guiwnzlpc.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gfykbhyfm.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gwcrqniqd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gfzgbldiz.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gkvkwbaoo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gybqnyple.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gfuyqggkz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gmbavnniu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gchqqaghy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gphanitey.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gsxxnqjvw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gjmfzzzao.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gguogezzq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gejqczzxy.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/goloaeyms.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gcuxpurao.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gbldqoolr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gpxastriw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gpeioscgv.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gzxuapkdk.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gjqnemjxg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gawheqdrk.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gtkaedyaz.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gkulkeqtq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/glprsomto.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gfgyprgjn.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gkrrfdzxj.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gnoudknwi.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gziizwvlz.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/grlceepqr.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gcbxzzffb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gwepegjmq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/glcgwbpiv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gdenicugw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvaxsjxex.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gfmzgsuas.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gwrzgugsj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/ghdruajwg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/ghcqjmdne.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/grhfokcjt.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gfwionbym.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gcvslryxq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gtbflutyd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/glorvvxwk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/ghwdztlln.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/graxjjlun.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gbwoguiyr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gzeuneqxt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gmtiwexyu.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gikyauboz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gvhmfwmtc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gnpbopdcc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/ghblkpqqa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gdivjuebe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gcnchixxv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gppebfwoz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gaquinqyp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gguiqgwwg.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gxpqllpvs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gmjzjjxnz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/goudtlfpi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/glptbyiyy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gptsttsxy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/ggdfnenof.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gcczpeoub.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcddapfpx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gtimpyspy.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/givzbrbve.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gtzwykvtu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gztwnewvc.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/glblffsbn.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gutuwrxdb.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gpvsjjvhj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gowbyqgtb.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gyouaqxth.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gxprglehz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxadhcusc.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gdidamxjd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdnploiat.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gbxwpyyia.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/giyszhydc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gteuksxuy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gxecaasqd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gfzojdnfq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gwqftjljr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gshnrmivv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/grtijxxyh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gfedqwcin.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gvmazmiar.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/grnhocnlu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/goxdtzmty.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/ghadlvyjd.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gulsvxaqe.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/glgtkyxjt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/ghsexwlvm.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gjlwzvrhf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gcxwmujaq.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gjjspibfd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gdaaeknez.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gsbatfgrt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gjyzwgtaw.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gaafqutrr.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gemazycuf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gaogqtinb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gmmooeomm.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gvgpbaurd.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gmwdaamxc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gnkjkzcvk.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gntyunjsh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gwvkclvpe.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gkdggikma.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gyfhtjrge.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/gkgmrwhwg.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gpevjxusx.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gmhhfylzb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/govqplwgv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gsaimhwvj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gdnhqioxk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gmapakbvj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gahhlrmps.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gbvpmbhuw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gookjchhj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gsvgvkozv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gaagbqghw.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/ghjerqsyf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gpxijcqru.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gcnpplidn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gszddnjdi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/geddgqvpr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gvmojlfdm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gagpkxkas.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/ghifevzwn.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gksirozns.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gqgvzzgqv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gzhsqymgv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gxtlauend.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/ghaaopigt.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/geuqzedwg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/ghyzwzret.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/ggopjkeic.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gmgaxklrk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/galselfca.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gsgwucovh.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gajwfhgkl.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gznonqhcl.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gioahhqbg.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gwststfxb.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gqfdxzyxj.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gdxrfeduk.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gtzfabcrv.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gggjehwew.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gbqndpvnh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gwywyttka.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gtuehdoiq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gfkitszez.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gtefribcz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gfutnjpfl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gtmlwktzs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gwfaitnyj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gwsvxuwjt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gfcbrwawh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gcbdqfbzy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/gedgddqxf.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gncmqnbqv.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gkffsnxdd.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gmqtijimh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gkyadgexk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/grhkfsqge.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gntttbjet.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/grgyigcgp.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gnwmyfykt.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gnqlowvsk.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/golwhybzg.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gfvckenbw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/goknxwoou.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gzacxscvt.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gbgslwxwe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gokvdxbeb.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gipdnxcgm.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/ggblvwsmi.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gvrgwduse.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/guxwgflgf.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gmhmvpqyd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gxgrdsdcr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gttrfnfwy.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gzxaxgioq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gfvkhchmx.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gahcllcbj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gtyyclkcs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gxcivamxk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/ghkqajhvk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/glsyrpjyk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gjszkszsf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gxcagzivv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gotfpvheu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gvrehxfgu.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gflleklre.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gmszistdn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gpguhttoa.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/glccmgltj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gszexmqwi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gznxelxjj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gfuiflvlb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gfqegjgya.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gvldylkst.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/glgebsgwa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gdwleuotv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gzzxpbabi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gntuhbboc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gcjqmxhnm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gksgmvmwt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gowxxqtyd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/giqijvxel.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gsnwtskpw.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gandphbdf.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gytiecqdu.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gtohtkduz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gspqifxef.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/ggvrweefn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/guegxidoc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gejygpnvr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gqzqjjapn.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/geyuwgkcl.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gynpcgdxv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gvugattlq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/ggxjgpegk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gebiqlyqs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/grvikpfbw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gimzbwjgo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gdxhntdkf.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/ghhyztzzk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gwavarlss.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gkwfxfiaq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gsgmfacdc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gcgnfroui.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gjlnvphkd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gkbphjddk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gnfnzwlst.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gpwvdsmyq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/grwwkkgxl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gcowubqzi.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gkjatvhim.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gotqkwbuk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gifeskzhw.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gfhximcku.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gyjjeitfi.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gvubccnil.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gtxdlqonv.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/grcvvhgzs.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gfjvelyvt.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gbjuoipas.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gtegjegzt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gqxvnclac.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gqkhrlcnt.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gicndahwo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gpwrwmguj.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gcxpnwlnu.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gervvvrxe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gastkxuoa.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/glwsfboax.sHtML


<!-- 参考信息 -->