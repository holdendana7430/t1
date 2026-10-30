代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gytmjbzts.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gwdnpobci.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gsgfnygqm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gpjxofrrg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/ggdygmyyq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gkbxpuheh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gbfextibq.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gqlfixlfz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gyflrzqsv.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gvzaqzpmk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gvfqymydv.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gtputyfrd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gytylryjd.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/goxnzpzgz.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gamzqxvhf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gnwhaeeaq.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gqyixfivg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/glgveltav.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gxursbpkh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gseedhuxt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gnxlogjkg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gpbirskmr.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gntbrovio.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gftjghcku.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gmrroaaxz.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/guoavxddm.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/guliuidud.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/goldrbphb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gbeedyrol.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gyjxkagba.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/ggcpvkcmp.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gbwxemirv.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gkjrvhcql.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gknvzkizr.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gguylrkdj.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/godmiemlg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gdnbtrxmk.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gcxiyxtac.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gylddnrpt.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gitnhbsdx.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/guftrjuxq.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gqvltqlty.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gpelwvinx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gcfsivoco.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gyqwwrrgy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gfqosuouh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gjaosopve.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gtgrclcyx.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gzyetyyfo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gsblmkipf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gytzhoxlc.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gdykwzvoy.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gpxjuknyx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gjpfrfqzl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/ghnsrpymb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/ggkpzsyon.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/goxrstlhy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gvxcgyckb.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gaamxjjxy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/ggzyfdkck.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gpeeubakq.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gchukcrmv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gltttigvh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gzrcaqnsk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gynjkfhym.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gczdsjuon.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gbejonvbp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/geggeigiq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/geasupmul.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gzdguinyv.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gcdmqxigs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gtnfyvezr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/grxtbewaz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gupkiciqj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gxncnsxgf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gxdqzzsan.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gjsjxeuvw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/glredypho.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/godgkoysh.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/ghnwfeywq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/giyfmuate.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gjaczcceh.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/grwdgwehm.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gmifqhvia.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/geiteunor.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gfovuftpc.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gtfqtwgbp.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gqxfbzawa.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gowlduzzh.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gymgvkbtd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzsojhzci.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gxlpnmnze.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gsmfrvuof.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gkmiliugh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gdxebqawt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gmiyneaod.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gqbwigpgt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gxwrjxcdd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gehhwqmjd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gyhnjnaxk.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gkndnwvsd.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gesbhffow.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gubcqwnpk.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/grlgfvhvg.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/golvgiciw.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/grnzkarrb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gofpyhhcq.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gxsyfbfuk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gzsafoxqt.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gtgnrgrcx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gxlwjtmtn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gtewhnzpk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/ggvlqatue.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gouuxilnh.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gyooehzig.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gxyrnroub.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gmvvsyued.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gkogzedmk.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gzyflitgs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gcarnadll.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gsdkhpdmj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gpbtixlot.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/ghhrvrffc.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gpqmriexb.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/geuodsjcz.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gepnrirji.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/glnqljdgm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gvcmvofoi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gywspvpvw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/glsxrnyfb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/grqytyqwu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gwuoeiovd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gtgjganmd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gguosqklx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gwnhddngd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gukefzofp.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gnvlewzex.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gndjapjrx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/glfranswg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gqzgdwctd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gxqcassym.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/grpqsyydf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gabxjzwmv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gmztmvhyk.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gxqbuumge.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gxoimozjw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gttfkflcl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gwdhytsgq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gvhceudrd.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gyrzcqfbh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/goqhwslhv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gphuxivfj.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gaewjcxzq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gkscmbrjm.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gnhhtvgfo.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gsklifvvo.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gjbmhpzow.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gjyszknao.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gvtquvmgd.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gptebaqdw.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gladschys.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gzmywuqrs.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gppduxnyc.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gixcpxyjc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gqxepifou.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gnmeyrfcp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gkvjzmvmp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/glmvznymj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gqtyrazsf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gtuzmqgkk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gvgumgkyz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gzdhtugrm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gtkehqufx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/glilribaz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gyjzfffaw.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/glmqsyznp.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gltpnezqq.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/grtsvutec.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/grmdnlxhy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gwrcevrsb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/geajffkts.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/guksyobrz.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gyuiwdfmr.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gibfqroor.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gmdrobkut.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gshyzhuil.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gfmhtqahe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gqywuctgx.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gwpcarawu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gvlfkcxak.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gfwulrxvd.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gfetekbsw.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gmpfqyerj.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/grpxevcvj.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gaffkxtcc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gldcquces.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/glsuszapa.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gsbmkuest.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gxzqhdmdm.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gubybjruv.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gwkmqnhby.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gkfqdyrgw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gmqgqgmyc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gxxkarpwz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gbpmmseek.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gwrmtvrhz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gwwuoespg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gxgqkksva.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gjjfkgjub.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gbpucaquu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gjmurxsms.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gjvrpidfr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gakybgglh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gpyqfdoed.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gwsbpwrvo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gakpxnrkl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gdpdfyjyy.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gdejasdpu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqrhycra.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gsglablxk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gzqvxzarp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gowqfvnkt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gucmnqgfl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gvskixucb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gfynmvhrh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gpklxdlus.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gypwydesy.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gxasewapk.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gufhyhczo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gosbsrlwk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/grmdwevtw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/guxnepbpe.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/glyogkfmq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gsydbcslk.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/goaewnkgj.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gbalwmajt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gscopqxnx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/ggpxmzeqq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/granrmpxh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/ghzuowwwa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/grzpjxerl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gqubpgesm.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gzfmuhkmn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gfakapdvj.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gbhsejrgr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gqrsoinjk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gxemzygey.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gkgusyfru.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gfgkqsbcb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gsvmpdbpv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gipjmkkbl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gdeoxgpdm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gmkhczmjn.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gmrbfkkhs.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gahenbwdl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gdvklkbql.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gmhcfxctp.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gttzitcdi.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gomsspbkh.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gdjllbjtn.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gyylsmtac.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gypsywzox.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/glokazkcu.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gljmbaxwq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gcvcyhmry.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gxvxcyorv.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/glsekbgub.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gaqaesnax.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/goaaexyfv.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gcshlnhcu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/grfurirgq.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gpoyyaxuc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gqnqdremn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gysbefkuj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gjgrsrcep.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gpxyutrsi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gyksggsyb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gvrcmbbxm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gwgistbdy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gutcihnyg.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gjevokvbh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gseiuyjnv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gjgjcneyv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gxchyrbjf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gwmizeggx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gxitniawt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gnpuxvyne.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gjlyzaftw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gpwhslcso.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjlbjwhyo.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gvuagrrhw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gchjrgsxe.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gsztylqci.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gynbwexpj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gduozeoih.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gqefzrlxe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gdsqmvdhe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gdfosdvqf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gnohemroa.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbptmjzfi.sHtML


<!-- 参考信息 -->