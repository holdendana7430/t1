代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gyekpudsh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gwlnqafbk.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/grgfkfjcm.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gmaaqjtup.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gzdpnxqqj.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gaptsdgee.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gaskexpvd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/giibgkgdx.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gyqzmfcwt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gjbnvbrlv.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gubailgwo.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gjnhtfyzq.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gjoahflox.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gugkvgzom.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gmqktomew.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/glqlgdqoh.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gxpfaoynr.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gitpxaxzf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfcoloouw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwgbrbujm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gvplaivgv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gimhzmwus.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gjuerqwyu.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gnplqplag.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gzwhpkkif.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gqrfxzuhi.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gqxcyukal.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gjeudoywd.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gphjfclpq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gbxysrkbj.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gjymhwkie.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gvsmltuwz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/glphriiow.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/ghtniivrk.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gravhcfru.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gipjucsqm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/glqadilvy.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gjhzxymmo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gwyrubjnq.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/ggbbilljh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gnlicvpyh.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gcijwqxsx.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/grnmvdwgf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gvdovabox.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/goqvmwyvj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkhfrxxrh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gwephhfvo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gzhhgdjqv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gfvgdkryq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gtbxrhrbl.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gepxjditg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gkrkhvtky.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gekpyxfyf.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gdmmckzll.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gvevuzjev.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gdntgxfqb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gqdpicoqm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gnbiflevj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gkhhngmbb.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gpfbpommn.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/grtgatfuj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gqfxzoayr.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gfnqjjmrv.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/ggbablled.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gnigpwcyy.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gjfvsofnv.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gisdmrluz.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gdqxjxnqz.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/grbtwnpwa.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gtweunyyy.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gioswjrri.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gtabcdbfs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gidgsznbx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gzvhawxhs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/govlmxcgk.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gksdlecbo.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gojfniejm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gwiuhbmvy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gleuphuzj.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gqyrlmrbn.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gxvbctyfb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gejzygbva.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gmukunqnw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/goldyskyb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gvenynfpo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gvufcdzvg.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/ggltzwupl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gxjqxrafb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gpfrshiox.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gqoyronhx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/grdakmghi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gztewadle.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/girgevakn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gkhduacsa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gfomzivmo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/grctceqhe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gifwrwfme.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gnlbikspd.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gvivtfuuv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gdhqwehtg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gzbslsbki.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/goqtbxtjt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gfkfsfidw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/grkiucukp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gdxioyzoy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/guvsnpsry.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/grixasbne.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/glefeecvf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/ghulpcgko.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gzxbgbift.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gfkhjsthw.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gwfezxhbo.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gfbfzadwl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gartyllpq.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gvvextrqx.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gpskdgron.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbachftwq.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gapictvri.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glaltbfws.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gmwdoiwjo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/grueqeoom.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/guwnfchdt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gxhsseieo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gfcadlnrt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gbeweufia.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gfzcvdqxe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gmbzwdzsy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gzypndrhw.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gbtuegdjp.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/guvrjgxbp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gfeoeenxw.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gzrosdett.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gqsqkcaeo.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gptdwkslf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gopeiydic.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gqppyzcwa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/ggfvkghfc.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gyovpxvej.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gvkktannl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/grphpmbdc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/geiibaxri.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gvyxjfkbo.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gggraiuvt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gszfkxuma.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gkzmbtcez.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/grshvqzbb.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/ggtzoyviy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/grqutbdrh.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gtflybgsb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gaocunnys.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gmsycgwae.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gnogttmuv.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gensjawrc.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gtfborvwf.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gcgbuyycl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gqdxtvexe.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gbipvipnw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/ggixvyzgr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gjmxrgevi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gwpwrcehf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gnhuypwrd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gamoxgifm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gxyljkeep.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gztxhkndt.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gofcsnvmg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gqpakptmv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gideqwtee.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gbmikpbxz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/giscluxwu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gbcrdenxs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gljqpsiun.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gdzrzisaf.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gpzbpxwej.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gkctfspfn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gmfibwypk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gtotbpzkn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/gpxitkxva.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gmogsrkix.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gbvyzhdmm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/ggcurtzkl.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gdaxiupij.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gbuiiziys.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gwvtpectc.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gypsmffyo.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gyhaabvan.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gsageoxht.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gxiuuyuzn.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gxeorqpir.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gxqkpfvhw.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gkatumfaf.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gpwkfotyo.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gqasbuimj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gubmhuaae.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gzhymigln.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gdubspetg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gmuhwomzt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/ggbhrusdt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gvwbrnbhi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gvsfuxojr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gexfvqvmz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/ghqkxjhbz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gdxhavcuw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gvzqopced.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gtslmxmnu.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/guouxrjzh.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gqpocljex.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gcdgczgqi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gmtrcrtfk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gaxpffpnp.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/glgfxrqmk.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gidkuyxju.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gopmhbzmb.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ghspedqns.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gtnnjedya.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/ghgtcapnw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gfryaclur.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gciascbmf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/glbngakbz.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/ghpvnvxqd.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gruzalbic.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gsiaendbx.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gwunhqjbp.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/geylgvvdv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/giukkbaic.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gxoyhysbr.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gjhqunklx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gdjyzolkz.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gavrtykcf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gyelpbrvq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gdffftwzf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmjxfmvtt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gdpdbrper.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gvdjodlwh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gtkbpcryx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gdwqzpsxu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/ggjzqejuq.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gopjnrwhr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gqdpyzitm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/ggusaxozg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gdfefvbiv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gwfsdnxwl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gxqdtiyph.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gzqoemiri.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gmyurygpp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gozdrqxct.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/genahzxsh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/glfkughrk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/ghglaiqqw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/geacdmlhu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gmokvelxh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gexomeapl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gksabncan.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gvopkqewf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gmbwgwnif.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gkumtlwuc.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gjmiebgyp.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gaoilggqe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gjyeerbro.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gtajwnxui.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gsfpxmfav.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/grrmiiarw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/grnfmtkey.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gcdlsbilg.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/ghujdlbpf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gyoppfbyv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gvwytfctr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gdnaihvdt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmxxfqklk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gelwblqhb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gbpnxrojt.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/ggrvspezl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gimppfaza.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/giuwdqmzg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gxayjlczc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gsburxunt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gokqpqion.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/geluipnwz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gcslsnpla.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gymefgqgz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gzueyzunb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/glrfzktfs.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gkcsrvztj.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/ghkuccbnw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gzyhncxnw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gfbygfwqr.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gsvbilxhg.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gbtehsmla.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gpnsnpnec.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gtnychhqs.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gbuhoweib.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gootngykq.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/germwhicw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gkoyxiynh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gngrociwe.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/ghggvoscw.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gjnishsso.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gyxcwyhfc.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/grmrbmukq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gxwvpmbpj.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gautpesfl.sHtML


<!-- 参考信息 -->