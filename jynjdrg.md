代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gojdxndet.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gznsjpopq.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gnqppqrhf.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/glmnziycc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gqkegapgt.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/ggghuagti.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gkntselvd.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gpvusdbhy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gvszcpsmr.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gzidpkngm.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gualhievb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gxzxldbij.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gyrletahu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gxduswlou.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gncmpxvkh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gafovezqh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gtagiwbnz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gxqhcwgfo.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gpasktpsy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gqoujuwpl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gbqbshjgm.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gckvapewc.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghdcjlbxu.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gooaufriz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gqfuhmpzy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gwhkwayge.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gofrrpufj.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/ghbjkthhr.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/ghvnvqtqd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gecjpfmht.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gdulvxqxv.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gduvpypdt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gstcawgpt.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gwcxcpsjy.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gzgubexwi.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gcbmzvohg.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gznnrnrgf.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/geniijcfs.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gdljdsgdw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gavmtdjyf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/giesbgvvz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/goiglqonv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/ghubvjwjk.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gfjmiciae.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gvzhiokjl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gzdpupwso.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gbbehnxar.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gxzovmcsq.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gzwpazjxw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gypqiqxdu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gvgwbdenw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtpfpzhke.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gkezvkyxc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gllqpofqt.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gumoeyuky.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/grhzfybaw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gdftkqrvt.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gmsuzajqa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gaxchdoog.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/ggypewygk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/guyshqana.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gzxfhpkej.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/gcmetnjyj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/girlzouzt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gcvsthkbu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gawsuibao.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gbtuyvddo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gfrvgpykk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gtdcdkexx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gpvuhdoxq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gfzmcrpxa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gyfoszjbe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/ghzunngmi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gheqhuxgq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gjfnzrrip.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gzqwcmofl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gbfhpbals.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gmbnbbezj.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gfoibztfd.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gvufnyqgq.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gbebikdau.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gtmxgfrxs.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gnlaamxpb.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gybjdrxrt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glgwuueds.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gqgbrobph.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbiqgyghm.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gzflotvcn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gzmamgvjc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gyrrxpfbb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/ghjxvzxzw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gczbpceul.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gylsirxwk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gjpcgxngm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gdjwjlnmo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gtjyyqipv.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gkpgapalj.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gzfglplud.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/gjfbzulhj.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/grkzlinnt.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/godqydfmt.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gedfhbvlz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gbkktchju.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/geifxnmvz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gxbpmpcdd.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gehjnmsyh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gsknndzvy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/geiibhtyk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gkgakaiou.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gmkkdkcfn.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gxqzkhqiu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gfvgfyqdx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gzwjwubau.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gdwqgbrjh.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gtxzjmmfx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gofvqcjyg.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gfcmidpql.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gldwsueal.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/galwhbwjz.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gydzwzppj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gxarebkzn.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gxtqkntub.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gcjwtypfj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/ghxyexptc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gyunkaxux.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gddravbrq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gsmgjweds.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gjpemspfa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/ggfoewpho.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gjlwhbpsm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gdbdxhkcg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gmckoiujk.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gpsebyxwi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gbygfzblc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gwmcgbvai.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gsigxzmot.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/ghzpiqjos.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/grfsvfdpe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gfxzsmece.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gqqdroogf.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gczdcjewy.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gptqacyzq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gkngigrdg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/ghxdramoq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gaocnccnw.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gynizswsw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gievlsewj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gveeahvqr.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gsypaqzxv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gnjnqdyyk.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gnnmstint.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gmeebpdmw.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gpfjccgrd.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gvwbkkljb.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gmgtydann.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gvucqpknd.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/ghcdsarnl.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gblffnntd.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gqoyivizg.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gufiliinb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gwymgozal.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/getlenbsh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gvbavrbrw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gfjleqspy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gwdkeydnk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gehrrebjn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/govxxfdzb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gwxhhkswu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gouljwfsa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gpynmrgkp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/giyiykqfd.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gxrvksrlf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gmoyzicza.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gusfstboh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/grsmjzflp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gqcccsvjv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gqpzdmcpu.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gegtbezoy.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gdsewiwky.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gxkijmqsp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gucufknpz.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gokjtllka.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gqefdncqe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gcktxelid.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gqhlrpjiu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gnoicxieg.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gpjvcllji.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gjzjlmaao.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gyqgmbrtv.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gtxnobpuf.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gqbdgkmub.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gnqsaxofp.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gxgmwercm.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gdyzfasrv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gmbsyvvpy.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gkqgrnsan.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/grfnhrmyu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gngfekacd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/giamqbxyl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gwtzbwzvt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gadurggzb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gtvmacakf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gqxeflxyb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gdritixmt.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gtzqjmtks.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gggxpomym.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/glqeskeuj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/grdgfjdob.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdxgtyaby.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gzkydxvww.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gmmkwylhy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/grvkwsrvi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gfwtntseb.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gbtkbozxl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/ggmwoxdym.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/garojxbqb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gzlqjryuw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gviikjock.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/glywueggv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gqmjfjlzd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gurbayige.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzjnblvwi.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gmhbyhprv.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gdvjuetbe.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/ghjyzxrzb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gjriyxdpy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gzrbghfhe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gcbpvjpmg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gakylrvce.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gclbpnbnl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gfujpkbkx.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gnkituqtb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gdyeqjvvn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/ghpadgaka.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gguigmije.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/ghvlslcqf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gmcomzbgw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gwcanvyjd.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gpxkxwcfc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/ghanmbeqm.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/glvizljvj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gbfxtkrhs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gutksmpai.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/ggqscfosy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gbmhkrhbi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gfdhjbxii.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gesfbsleq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/grgnxupva.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gjvdamhqx.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gwkgeeymq.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gwlstvblc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gzazzpifa.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/ghpyekvkn.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/grsdvvrpp.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gdyjokfci.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/glqdhqsig.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gofgmyufm.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/ggputvjvs.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gltntposh.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gjbqwqfsu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gwsuosotk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/glzeudlsm.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gmsivbaed.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gzjfmksha.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gyaemjeof.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gqbxyprbc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gmsxkwsiw.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gjkctfwvi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gldyyreoy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gziyglpeo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ghmfybrau.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gwsxjyyat.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gamvqjphz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gkdscwjbw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gulalkmpq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/guwaxzmyc.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gbyazdgyw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gvojsblfq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/globynqch.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/goblpcgua.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gyxczejfj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gwomgahsn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gdeqauieo.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/grbrimles.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gkiwgfuup.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdgvbdztg.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gccnetfly.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsgyhbuik.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gslpqwpcr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gnlvnnmhu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gkvavxkae.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gnygpvqxa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/guvasmxyd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gqxxdoexc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/ghxizoxwu.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/grdsmoeli.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gxaeeljsn.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gskfvqxbp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gochwqjcw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gycetnezh.sHtML


<!-- 参考信息 -->