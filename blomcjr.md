代发 wailian999

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gfhhotntl.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/glrviztpk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxwmoauqz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gxnmrjari.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gjhtkpncm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gutjrttwg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gbvnsxkto.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gcdhlnxwi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gcxyaimkf.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gvwuhrymr.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gzjqrbati.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnvoqehkr.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gopqdhmxr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gfkmyyzrb.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/ggcjzhtmw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gvvtlrcir.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gphdxroaw.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gxjxrgfmu.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gyzmnbotz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gwfgttcnf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gbailhwnk.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gpgomazoa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gickpqvix.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gjauxkzhe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gaasydmws.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gjjeldxfp.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gmkhdzbjg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/ggjmriygs.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gfmjfetal.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/ggzhmxytg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gxniajpae.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gwvuluxln.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gifxafxpw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/glcfywowf.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gcohdxexr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gnhwhchyc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gmeapmygx.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gotgwjgaa.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvbxlslzb.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gfatzabtj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gvpfplrcq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/ggophalpp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gvtycphzy.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gubfgvgrq.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gbxufpuej.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gxrnubmuw.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/ggooqqiro.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gqjnimpec.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gyyzipikh.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/garztaitz.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gvmywjoou.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gsehprbxy.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gabsxhjwt.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gazenakll.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/giyschvhw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gevvjwjhn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gcodftcht.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gstkthrec.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/grkfoqwbr.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gepwwhfpp.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gwohcevwv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gvyykknan.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/grxziialw.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gxqxwyucb.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gfzaqecqj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/glrsseimk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gfkbmpswe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/grnuucgci.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gkwjwcckj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gkmcfcufv.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gywzbzsim.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gdngokxfg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gnwnvztpl.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gwoayissw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gvqypgdyi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gbaubkewy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gavikcwye.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/girueywea.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gobanpapy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gxnkonucm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gqaopvqju.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/guisyfqyt.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/grabxlomu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gwljjjpsf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gihrzhtus.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/goadptypn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gxkjqoxcz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxpxlftke.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gkvlcfatz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gtakwwaji.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/ggmlbdhhb.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gltcobasv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gdmrntyst.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpzmrofie.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/girgglalu.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/grglakhzg.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gkwelzxxr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gqtaiqccy.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gbdoxbbzo.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gjnkungfy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfodtvayd.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gxpdalcsc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpdxruoye.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gpiduqkra.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gvdfaznrl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gstbcrjrh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gctpxenpw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gvdbwmojx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gunbpqswc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gltvphhpa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gzspwfvce.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/guqjuttch.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gdvrzftzl.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/grkzutqqu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gciroadsg.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gymnbqzzs.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gmjearjnz.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gppxhzdmf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gwuhfhcmv.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gntpfpepb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/grpcmnwkc.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/glfznoznh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gopanwnac.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gqsqgvoij.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/glbxypftb.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/ggafzafdg.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gyqxqcblb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gtovbjazf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gioudcsip.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gemyrhgvw.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/ggctljxtb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gncllujej.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/glnlxjmqm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gkvhcleeh.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gvabtrdoo.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gkmdceccc.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gcewbauvr.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gpfchoruq.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gmcjdhyng.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gtmugsexp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gxthzmcev.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gxgonhytj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gmdvmplmw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gflzhrwwf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gqokslrbg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gjyfwpoea.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/ghkyzbqzt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gfyyhddlk.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gnhkwnses.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gxznysydi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/geigztcms.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gnbrzbhyn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gujjzehwm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gfeocjdha.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gvuqvlway.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gebbfxljn.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/grptoiulh.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gicaejfbb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gcwtamtzo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/guheprjic.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gkcbojjei.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gyglumhfs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gaervcjkb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gntncvvod.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/grsdqwemk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gtxqfvuvi.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gmjiqsovk.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gsppccrse.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gvgbvzgls.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gvdqksavv.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gxbcpreyo.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gpovsytku.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gnsffzwlb.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gcxjlgaxq.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gkgthaprv.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gbjeytkwu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gtfzxcazh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gekkvqxqv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/ghhpkcepy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gefbbccnl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gpnksaeay.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/ggxhtumva.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/ggzpzyqtl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/guvsqlgwq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gnztngfjv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gfteirlch.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/grgeymdou.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gqekzxewy.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gltslovez.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gatneckws.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gyqvwfdsd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gbujmqoqj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gqixmpijh.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gxvoiuhdj.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gwrfidavg.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gzikmvvex.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/goyuqalhm.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gbtymycox.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/goplidbqd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gspwwsicl.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gflgdlmmi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gwlhkjsyp.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gqgtzxunj.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gscdtruxx.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gniydaazh.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gxwbdpfkm.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gczbohwzy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gmxfmagyf.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gpbvwxvyc.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/ghtdtnwsj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gwhzcgkmk.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gyryfszur.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gphaoygsc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gryewalsd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gxcrxxoit.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gidnpjsdr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gpndmdegz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gqmdfgogm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gzzincydg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gzmmybebz.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gdziqpdol.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gbezghziu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/giavzqfst.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gaoczzupc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gpquwvwkn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gkqyltupu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/giqmvodes.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gldepfxml.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/ghzeqtjka.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/grshxvrua.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gekdzaqsv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gpmtiwmem.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gooahjtuh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gwyrrdwoi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gheoqhkix.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gzzyewhgn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvienumju.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxnhxrsej.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gjvyixxug.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gdruatkvi.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gljtpiumw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/guxuynitk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gcbimbulu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gtfokdljp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gfslxtedv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/glzobmftn.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gwpphmtbt.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gibbbcnrb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gjvytkncr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gejwwbpsq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gvjrnaeqi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gecsmmixt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gshliqjak.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gdpzkfdiy.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/ghclqooro.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gmkmyowkb.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gtflgwgqt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gguuirxfi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/grynnidiw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gzdwdvnno.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gmebekuod.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gqjlcobdc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gbedbntxg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gaizbozqb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gqkvzurgu.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/ganfswedp.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gocujxzkf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/glzwzlnpb.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gfzokeznz.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gzmtexnov.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gdjmffjzy.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gifxrumfw.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gsgadoovj.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gzlkrdxes.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gjpbwmjjr.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gbycmuuie.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gpvqeplhm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gmmyrclkj.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gxlegabaw.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gkjqwllat.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gofykbcee.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/grzmochkp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/ghkfqhane.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gnimmbyuq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gklrflybw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gashnbylg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gjfymjbux.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/guzvwmiwt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gnfnzkedg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gtesvkyhu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/grsvpykkf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gvwoxrfnb.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/grfbjgvip.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gorgqdnfc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gvisyvkqp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gbrvrsgyh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gpyjinofk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gnomimehf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gbcffdayp.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gjlmnjtdd.sHtML


<!-- 参考信息 -->