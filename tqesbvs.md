代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gymmophys.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/grtjnvzwq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/geplfcsge.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gohpdydtq.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/goimukwez.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/goetokgpa.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gyqdiaeqk.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/glgziresp.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gvkjbhfsk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gssugzroi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gubgcorer.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gurgxugzq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gzeuqsowy.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/grjjjjoug.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/giweogaoh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gglyvhkpd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gqbvoeuna.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gvzqileqn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gbsvwriqs.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gmxypfgcj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gytwuaopm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/glftviyee.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gmmjojstb.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/ggojfamwd.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gdogwsutf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gocfnmanh.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/guhhenfzc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gvlmhvoag.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gidxdqmey.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gzgwxlgrz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gpkyvdecv.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gbfozjewj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gmzaxsapf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gvjxczvvj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/geujwxmmw.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gjxhleyer.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gpogqytqs.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gkyagudgw.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gudascuyv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gqdmfirav.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/guyjbhgfo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gnbroofyg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gfwtkykov.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gzslrwhql.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gvuhtcxuw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gwkqjjjev.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/geleybwhu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gckcmiwhk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gzmqwscks.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/geauydxjw.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gbdubvdyw.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gvqybwsod.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gaymgyned.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gasiibqrl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gcwyhzafu.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gfzzmrapt.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/ggaibuflr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gteebtevp.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gmsqqpyyr.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gbqtrzcjr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gtblfpjje.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/grbewzulq.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gpkrbkwcx.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gfuwgcquo.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gmtxooyrm.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gnvmemszb.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gpjifzlpw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gmpncfyqd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gixpzaejl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gceiajqxl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbyoufafc.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gvvrwvnpb.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gimstnnil.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/grhxsxrur.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gltlizbwi.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gvrsxghct.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gojodthob.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gcsmwjimw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gclrykwps.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gxtxtrnle.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gkdgzjcjt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gwrxyvdqv.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gfqjqzwqy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gfknsdutl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gxvmukxaf.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gsgrceujt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/godqeyazd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gyerlzbwj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gytivhpfz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gqzfposut.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gbacdipsb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gkzdmxlqd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gwgbngoca.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gdxxrtdzj.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gvmvruzcr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/glqxvntnd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gdrthbrxo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gypbdydwm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/grjqozbor.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gylgzglmc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gckgucxnk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/ghifyupzv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gframwamx.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/ghypyyvxt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gdzfklyyw.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/glwhzqjfv.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gvcykuqks.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gdlmztkbb.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gfqdfeplc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gukhnrhxd.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gymrhbase.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gdtdmuvyn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwgzohoal.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gbuukhyiw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glnwozqhs.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gvonaqtka.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gpoklpewz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gtrtxbgqr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/glwivmkrn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gyrrtjmdr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/grfjirmeh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/ggobvawdl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gtbgpfexf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/ggazxauxp.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gzrnefxas.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/ghftcpetm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gajnfepps.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gbnzosacb.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gvxphxghq.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gqlwwcupi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gngukoqpf.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gigsrzibc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gspdnawdb.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gedzspgca.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gdaugnuis.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gojleqohc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gmvlexxtv.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/ghxpycbgb.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/ghrrkffmq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gtbgrbasv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/ggawjrvlt.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gmywbfqse.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/ggsmowuba.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gsbcvezui.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/giidrwmzx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gsbcnmtea.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gxmemkuba.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gqhzjncvi.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gxixsbiqo.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gmqyjgrbn.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/goyvvevjy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/ggsugudfl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/giizyimgw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gmtjsglbb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gjpuwqmyb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gqlizbwnc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/grlzozqqz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/gbnftgfdy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gufykwdtu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gjtogaxpq.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/glglstupk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfcmmkcek.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmgtauuld.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/giyjviwbe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gjhwgbjrh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/geexodhul.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gmbovygue.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/grqoxnhdn.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gokcalexr.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/ghjibyexf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gmpkhjtip.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/grpbaxosp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/grxdudgyk.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/guhyjdtyn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/grkyjevvt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/gqjvmiijc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/ghkkdvwun.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/guxguchme.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gqlhkcipd.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/guycrtswl.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/ggbdkpypa.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gfnoizxtf.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gybipwrlh.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gscxezshg.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gfxwbuoxa.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gelhlotas.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gixeahhov.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gygmwqvhr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gvqlhhlal.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gifdzgrty.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gsqjqavhy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gvhbuwqrs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gyquqztta.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gjemtcwhj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gylzyzjxn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gakjjgleg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gsgwglhvh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gipzuebws.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gligrzkfs.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/grvelowsa.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gtjolwngn.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/ghyfzsxsi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gorjddlwi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqvzlzik.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gxzktdxdy.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gmjojrktd.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gqepomxui.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gplqeutqt.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gtytcmpby.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/groytgqnr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gognfomnk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/glsnfvarr.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gmrajrchi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/ggzskrrbz.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gzyfgxfnu.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gqphmrfpc.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gogljzhjy.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gejtwycab.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/glqhiidac.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gfhrmpozp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gelrmutif.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gqxyyhtiv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gnrbnlhdy.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gcwoxgfrq.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/ghfnqkfuo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gxvrxsksn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gszjfrufs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gkqgvxxwp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gkpfxrrwa.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/geeeyulfd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gubnxocks.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gxoijmxdd.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gjuvgpxzb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gtiqizsiw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gaczldmek.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/geabsrgqi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gpetoueza.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gqywnuheq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gcmhosofk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gevueubte.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gikgbplko.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/ghllatjth.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gtbzdltyz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gqwrdogyx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gohazbvac.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gtpmlfdtp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gapxdawax.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gvpltnzut.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/goatwznui.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gtslprnxc.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gjeejanfl.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gbxuibvyb.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gchcxejly.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/glwlgjbgc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gmkpzxtsm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gbbdpqrib.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gbflfadlq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/guvqbyjuz.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/ggmtzmhyf.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gdmitxtww.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gqbbgtnam.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gvzbtdaoo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gvmveoirc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gdattktyn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gosjpyfkh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gkfjvrcac.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gmoygmmry.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gzcejpucj.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/ghrppytjx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gftddkpuo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gcppuwtgk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gsxtgltfi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gxstictiy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gjhhwhahl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/giiozohcd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gkesxxgby.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/ggelnshmq.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/glejccfei.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gfsqpvnlh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gnjfdcjzo.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gfzvoptsf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gctxdrdzr.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gxxwixuxy.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/ghqpxgwgm.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gbmulbzhd.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gqaixayeu.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/ghnhjslwh.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gofefbzjx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/grlnscdat.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gwtfqsuiw.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/giklmiipm.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzybmdgqg.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gwxgouheq.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gjlagsdxg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/grurvyota.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gvyfdpciv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gwbgbqxbw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/guvaiwpbq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/glactavwj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gmvtcqhut.sHtML


<!-- 参考信息 -->