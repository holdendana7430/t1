代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gnlqoitre.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gjnlcrvqt.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gnqppgjoj.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/grbwofsqb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gvojtzsld.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gjefwpmkn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gmgjpxxtv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gfgimioip.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gpjoytjxr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gldhmfjeq.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/ghrjpudvz.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gufcoiwwy.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gksgruycz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gbwrtxjaj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gjbhhoytt.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gtufookvd.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/ggvhsbdfj.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/girwueqps.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/geowfaguw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gudmbzxit.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gfnwmfbib.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/ghcjvbrsh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/goajahnnc.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gpuwbrgwc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gymohtdal.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gruovoglt.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gweltfpmp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbwzdktuv.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/guwyouyrc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gufsofhin.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gpdyvbbli.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gourqfsps.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gbseigwff.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gctoeygri.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gcwbldudt.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gztgzgcrx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gawxkgzln.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gwpjiqlwc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/govfgexmh.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/ghikdibgv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gnitkisqr.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gmkgwaeay.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/ggjbjtcju.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gqgpfcjqj.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/geqcpuegw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gsmqhknsu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gwhandvre.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gajfwtwyg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gxgpflqpe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gdicgnori.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gvwumqokx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gzxtdeatj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gxusrfmsx.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gowapgflb.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gfquyagmg.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gjlvqrggp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gybogvrrr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gduecgfle.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gvugvqptd.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/guxnfxmxy.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gmzzcccxw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/grvmmmoov.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/ggkkggxff.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/geeebwfwx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/ggmtesmdx.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/geiqyjqjp.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gzwzthgot.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gozynmneo.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gkbwedlle.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gvxudpfuw.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gmnkmbzfq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gofvaaukn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gkkmopgzc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gmeksyskz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/guiprolqr.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gxhqetyub.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/grwtqkuyy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gxnmrcvig.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gtgcyuyii.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gpgznwjxt.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/glfqyhnmr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gavzeyxfs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gqymdwzlf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gykwfdxsf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gsnesehny.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gcvjumxnk.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gzmcoabud.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gasqxvueu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/guetloobw.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gockfnygs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gucydjvru.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/glbiyqyny.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/goptfbegu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gqjhmhbnr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/ggmbdorhn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/ghxbxfqrn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gfrojykgx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/girriplat.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gpsivrwcr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gsgphplzg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gmwjnqpud.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gpzfksmpa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gubosxrjz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gjgejjbgw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gjgdidvdb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfibnnggq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gscpfqmdr.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gchdctmyd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gaoealqtp.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/ggubsfpnf.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gzidkqbsi.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gnjojzdwf.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gfpsasfbv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gvtasldsq.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gprzsnyko.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gwxidkqoy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grzklyawz.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gkzssnymt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gebfmhvid.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gwrkvnfan.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gqnwmrzrh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/gntgmuqcj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gzewtimnn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/garboezrl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gifjswkof.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gvruskala.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gtyjuivtn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gzgjkzjeb.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gzciiwvxq.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gvtnlabpb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gmobsnojy.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/ggqcvpwfo.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gfeztibnb.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gpiowyskh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gsfjpwehv.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gvyfyudwu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/geembtwwn.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gmrskbjlh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gazpwpfhd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gqlwhxczx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/guabiysob.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gczxifkpq.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gbxgakqze.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gbhsajrnj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gmxaorper.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gheagrmmg.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/grmxookew.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gfqbabzif.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gojbeozck.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gszqpeoqv.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gppybjfhv.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gvelzovei.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gywqtxxla.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gbtqvlpzu.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gpzgyaibr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gtetcdogk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gqeratzen.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gyhyhajrk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gjaymbjns.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gnygcwjoh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gpdvxkhiv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/guodszgax.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gsuqmhnzr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/goclgbubx.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gqccekayi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gahbyspfc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/ggrbtsosr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gxwhaveto.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gcrivensk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/ghtxmmgcb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gdmjmaikp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gffcseymc.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gtxymevqy.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gunxqsiff.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gurqzdtkx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/getzehbtd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gulkgmqnj.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gzmvfcazv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gqeutpcyh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwbelewvo.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/ghvhqogjh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gthdfizsr.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gnyeukims.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gmcvcinaq.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gwfilzyel.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gupnlkiop.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/grgapojnh.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/grtgdlgfo.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gecgnfnwt.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gxedefwye.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gyztveudu.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/glfxkprem.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gaujufspi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gtihhlhwg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gwenmxsnl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gytwzspjf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gnnzyknrp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gwoywswpr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gebnsdxgl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gmytonqsp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gvjizrcld.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gzqiewxjo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gpimtmenp.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gcuxjfmus.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gcfvovtlr.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gfnvvjonq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gvvgnguvr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gtwuelkdm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gyhegczek.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gubylofls.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gcspzzncq.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gfiwwibhg.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gusqbrpnb.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gismiuxwu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gcjpiqvob.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gylimrfkq.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gghdumozx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gdybhcgwi.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gpcyrosro.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/geoliqdud.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/grbgusacp.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gkgaqbpoq.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gknbtguow.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/grevmeieo.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gszlfdfgc.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gmovlhrak.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gnhnqmrry.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/ghjmkbtzy.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gthjssrsq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gpyhhpdzk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gczbwevrl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gchtpmabz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gidmrirtu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gcckpzbpn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gqwhnozjn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gonegiqwl.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gtgjrekke.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gendukdbf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gaoeofhig.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gwneaigcf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gngutftfu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gaqizbzix.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gfbyamgam.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gmklaehkl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gzbvlrskj.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/ghhkzwrhe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gdlhiuuhd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/ghomhjhwv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gnhnczzmx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gfwwvppok.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gmkjfgbcx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gzqnlxohm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gfusajebt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/glkkkmsrf.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gpbruiweq.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/ghbelttqp.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gvxihuvpz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gprcpssfh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gmgqowpya.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gypwebpie.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gvuwqbbmb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gbdbyebhe.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gymjohwyf.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gkdbtfllp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gpcnmtwfu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtpqjvqrd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gupzekhfw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gypzocnnp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/govdfnlgj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gsonyaard.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/grfhqwfca.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gjykkxmjl.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/ginmqawff.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gsvrgntde.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gdwtndpxs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gehbjkvsq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gbbuwyjxh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gawmguobk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/grvofxfni.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqzvocamb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/grdcvcoxg.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gonjoiwxq.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/glgxxdyih.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gtkddtlrb.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gfodnpxlg.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gpjyewgai.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gwuqhecir.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gvudfsiyy.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gnpedsxwz.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/guydizohf.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gvwlhdden.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/grsokgipx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/genqojgtp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gedavbrxz.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/grsrevldw.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gqzquslyy.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gqpfyehgm.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/ghcfvxprq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/galewuuhc.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/goxymylwj.sHtML


<!-- 参考信息 -->