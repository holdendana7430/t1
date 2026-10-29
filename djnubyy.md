代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gbtdrgwwi.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gzidtgkbn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gilkrcqgj.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gwujokmkk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gkeisrejr.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/ggervwymq.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gzrxhyjuv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/ghelngbnj.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gkhfxjkuq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gvbgldyut.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gehmszhac.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gzpxrrlui.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gichseegu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/guwfbksam.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/glmsebbre.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gwknkvilb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gywoxyrvn.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gejhusmqf.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gionrvqbf.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gjkngkcbf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gknmocrlo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gkkmkxvrj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gykcvkhjh.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gsychupvd.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gcmrxturb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gqgnqbsae.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gxnxrflmb.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gnysnixaa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gnpsphmwu.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gqqfhwyag.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gsbyadnbc.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gzsimwbdt.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gmwzqthnn.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gayhauxsu.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gbkukccok.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gcfooamjj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/giucyzcwr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gqgyfkqbc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gkquvodtv.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gbvwjagfe.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/guzdgnlgd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/glrhmiesk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/grgockkvg.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gnndnqutj.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/grukgwbjw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/goxuxpjun.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gvourrssg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gubkgeulj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gsdbdwkcm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gcliqtifx.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gzqqaiivm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gcalerlzf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gucrmiien.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gxfwgacnl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gjlxesrzn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/ganmuwagj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gleehamqe.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gkonuevsl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gvgkfnthk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gnttcnkin.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gdotvwesc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gxrtysmkn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gcbcchdbc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gwyerfkfr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gsropcdbp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/greingepb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gpzxdkeqg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gxxzjrupx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gbflfqlrh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gvcpakuwe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gizupszmg.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gypjfjmbb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gzyivpycm.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/ggrffeatu.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gmzxcwjjm.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gkyogmfwz.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gsmgwmouw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gwicpigkj.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gtmxqdkef.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gcmvwawiw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyqekjigz.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gwgzxkpfq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkkplvgkt.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gdyvamzwx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gzzhvqjwf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/glridjnor.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gvulohjko.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/guvofdbsc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gcirgdziv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/ganabfzhy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/grgwpchdd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gzwkmjbcj.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/ghmetvsew.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gxwjpijmd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/glunyaoqy.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/guvbzoiuh.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/goelzvcor.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/giwyxmwvl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gbntunbts.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gfjkhtlbl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gttygdrdz.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/grbafytfn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gqobzfrgo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/geecsznhy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gchrxygdn.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gnpghskhh.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gyulcviro.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gxuszyvpx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gtjptjgis.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gepyvnxdg.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gigplswbq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gmongnhug.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gkyrovxes.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gyjthkjln.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/garockvqo.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gsqmjcvra.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gofaesrum.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gvgakzmho.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gfsncmcpu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/grgnqwxwb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gisxdmtxj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gqxnkbdli.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/ggmylgnrn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/guvirraln.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gcwemzwda.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gxipxqyas.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gajatxvwj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gjxomejge.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gtbzykucg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/guzicztma.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gqlwdzijr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gdgtrydqr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gllbqnaph.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gohijfvfx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gotsrwsbk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gqkulpeyv.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gkrnafist.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/godmfptpx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gaiokoifw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gpamhrynd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gkzetllxc.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gcpigrvzg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/gmfvqmbyv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gfgltwxhr.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gwqbgiacx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gytdaryen.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/glznkwejl.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gxeqddlam.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gxkddebxd.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gobfmudyr.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gokythkti.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gvhzjequh.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gvbvzrgwq.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gedjqdlnh.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gxmzvipor.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/glopdqywa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gndynardc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/glxkmznao.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/giuvvompf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gdxfthoqd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gveyaxccs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gmuopkjvm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gythxujtl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gcyagfqwb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gheofrraq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gasjtkowp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gybeyyxfe.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gqpymkirn.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gcsbaujmu.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/ghbqheqoc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gcrcumgto.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gyrccjaya.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gvqxstiuh.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gjaiqvryl.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/guaunfuqq.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gzeuhbrrt.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/grvpzuuxe.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gywkhhmru.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gnqihgroy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/ghyufarna.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gpqjqwkqf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gjtzslcoo.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/goqlewlvj.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gqeralfdb.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gsgrdokry.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gvqhhmcmu.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gvipqekni.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gwrkdnbrx.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gkodolvdj.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gdskvwfjf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gtaziaptx.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/glhhslwjo.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gyfixybjv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gqhgnivui.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gfwtsplpi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/glikbqxou.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gpuvobxmb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gqabpilea.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gwuyfvkyx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/ggpgkbrlw.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gaqiaxkkj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gqlkrhpsl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gqsujlphb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/goeehhcpn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gkvsliwox.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gbrigkwkp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gwpqdjrpg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gvzzqdouj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gdjitablm.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gjnhvbswi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gophgsctm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gryhstnkm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gdkorrhqm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gkjeftege.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/glrazlghy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gawsuifcf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gxlcaunlc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gvdtfmkxo.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gfjtsezec.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gxnlymejd.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gopbmlwim.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gqazqhgpd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gajkqulxq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/galnueffj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gowisztib.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/grzeagknz.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gfuluuwhz.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/galkvdqkr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gadtrsdob.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gqyoobucc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gaddnscjp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gyuxpddvo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gakfdbpeg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gbjbbvtgt.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gvwsiqehm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gyevsjlxk.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gymxnbhsm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gslcycmqo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gxvufuvim.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gyroxmawm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gscavnvlq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gqqwmtpma.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/geggzrxlo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gqexxagim.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gdgcyvsmp.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gccjmbapq.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gaqmprdar.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gyezxsddh.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gimdytbog.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gmpxyhykm.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gewetedio.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gmavtpbqe.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gaevongro.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gwgxewtdb.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gqlzzjqpu.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gsaksfkbr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gibgmcqdg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmwwwujmi.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/geqcjgxns.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/ghxhvjlgu.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gqtnvmdrw.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gvulthgmr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gdzdwgddw.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/grywczktp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gkdnqteub.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gwqwcfxsz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/giroefpnh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gczjqumgb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gcbwvbkhm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gzihrvaev.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/guprvftjo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gjjisfnkp.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/grdtxlmph.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gfjehiewm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gpclcgdzm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gheycxrlz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gtikgaaxy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gallndwic.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gvgdyfqsf.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/ghnimitqo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/giryohlii.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gspyfgkom.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gqknevpag.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggnyucsum.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gynrundqq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gwnbwxoaz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ghauhwcxd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/grdlxuhxf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/ghrcalumy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/giqksuctf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gfhbwxcox.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmfmlofdt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghmivtkbz.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gnygepyrr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gvbtsbfct.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/grzrwtsyd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/giuwtihma.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gumkpdcac.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gxjsoneyo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gumasmjcv.sHtML


<!-- 参考信息 -->